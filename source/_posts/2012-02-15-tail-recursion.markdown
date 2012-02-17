---
layout: post
title: "Обычная vs хвостовая рекурсия в Perl"
date: 2012-02-15 18:52
comments: true
categories: [Perl, Javascript]
tags: [Perl, fprog, Javascript, code, goto]
---


Написал сравнительный тест для обычной рекурсии и хвостовой,
по мотивам  ["Functional Javascript"](http://vimeo.com/35694483) (vimeo link)

Результаты на MacBook Pro 15 2011, Perl 5.14.2

вычисление суммы чисел ряда (первая цифра – количество итераций):

    tail sum(10000)   (0 sec, 0 kb)
    rec  sum(10000)   (0 sec, 5496 kb)
    tail sum(100000)  (0 sec, 0 kb)
    rec  sum(100000)  (0 sec, 45628 kb)
    tail sum(1000000) (1 sec, 0 kb)
    rec  sum(1000000) (1 sec, 476164 kb)

вычисление факториала (использовал bignum):

    tail 10000!  (5 sec, 636 kb)
    rec  10000!  (9 sec, 9612 kb)
    tail 25000!  (31 sec, 228 kb)
    rec  25000!  (63 sec, 15016 kb)

в 5.10-м профит чуть больше.

Боже, храни goto! )

<!-- more -->

код суммирования (факториал по аналогии + use bignum):

{% codeblock sum.pl lang:perl %}
$|++;

for my $n (10_000, 100_000, 1_000_000) {
    my $tail_t = time;
    my $tail_m = get_rss();
    print "tail sum($n) = "; tail_sum($n);
    printf " (%s sec, %s kb)\n", time - $tail_t, get_rss() - $tail_m;

    my $rec_t  = time;
    my $rec_m = get_rss();
    print "rec  sum($n) "; rec_sum($n);
    printf " (%s sec, %s kb)\n", time - $rec_t, get_rss() - $rec_m;
}

sub rec_sum {
    if ($_[0] == 0) {
        return 1;
    }
    else {
        return $_[0] + rec_sum($_[0] - 1);
    }
}

sub tail_sum {
    my $n = shift;
    my $sum_cb;
    $sum_cb = sub {
        if ($_[0] == 0) {
            return $_[1];
        }
        else {
            $_[1] += $_[0];
            $_[0] -= 1, 
            goto $sum_cb;
        }
    };
    return $sum_cb->($n, my $acc = 1);
}

sub get_rss {
    +{ map { split ' ' } `ps -o pid,rss` }->{$$}
}
{% endcodeblock %}

_Upd:_ 

Я так понимаю, что полученный профит по памяти получается благодаря экономии стека ([perldoc -f goto](http://perldoc.perl.org/functions/goto.html)), а процессор экономится, потому, что не копируется контекст функции при рекурсивных вызовах ([perldoc perlguts секция #Scratchpads-and-recursion](http://perldoc.perl.org/perlguts.html#Scratchpads-and-recursion)), что становится заметно при использовании [bigint](http://perldoc.perl.org/bigint.html).