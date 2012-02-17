---
layout: post
title: "По следам YAPC::ASIA 2011"
date: 2011-10-22 13:26
comments: true
categories: [YAPC, Asia, Perl, review]
---
Не так давно в Токио прошла самая большая Perl-конференция этого года.
Так как я потратил определенное время на изучение ее материалов, то решил поделиться информацией.

<!-- more -->

Итак, сам сайт конференции [http://yapcasia.org/2011/](http://yapcasia.org/2011/), для чтения иероглифов я пользовался Бромиумом (Хромом от Я), он довольно хорошо справляется с переводом страниц Японский->Английский (часть презентаций в html и там перевод тоже работает). Есть недостаток, что этот механизм не очень надежный (то ли меня банят, то ли [http://translate.google.ru/](http://translate.google.ru) "лагает" часто). Pdf-презентации, тоже не очень сложно перевести, если зарегистрироваться на slideshare их можно будет скачать, а потом все легко: pdf -> text или google docs -> google translate -> profit! )

Здесь обзор конференции на английском: 
[http://blogs.perl.org/users/lestrrat/2011/10/a-glimpse-of-yapcasia-tokyo-2011.html](http://blogs.perl.org/users/lestrrat/2011/10/a-glimpse-of-yapcasia-tokyo-2011.html)
из него я узнал победителях на конкурсе лучших докладов:

1 Fujiwara-san, who taught us the many lessons learned and techniques used to migrate his applications from an old datacenter to a new one.
слайды на японском: [http://dl.dropbox.com/u/224433/YAPC2011/index.html](http://dl.dropbox.com/u/224433/YAPC2011/index.html) (можно перевести в chrome/brome, кроме картинок, т.к. html)
2 Second place was Takesako-san with his Win32::GuiTest talk – пока нет видео и слайдов
3 Third place was Tokumaru-san, who presented the various ways to protect passwords in your system [http://yapcasia.org/2011/talk/56](http://yapcasia.org/2011/talk/56)

Далее список докладов, материалы к которым я успел посмотреть, с моими краткими комментариями. В начале постарался расположить наиболее интересные доклады.

#### "Perl 5.16 and beyond" - Jesse Vincent
Рекомендую посмотреть. Мне отдельно понравилось то, как происходит ротация релиз-инженеров в команде perl5 porters.

* видео и слайды [http://yapcasia.org/2011/talk/96](http://yapcasia.org/2011/talk/96)

#### Perl 5.14 For Pragmatists 
* [http://yapcasia.org/2011/talk/95](http://yapcasia.org/2011/talk/95) – слайды

#### Unix Programming with Perl 2 
* [http://yapcasia.org/2011/talk/76](http://yapcasia.org/2011/talk/76) - слайды

#### Monads in perl 
Интересно, но мне не очень понятно было с первого раза. )

- [http://yapcasia.org/2011/talk/82](http://yapcasia.org/2011/talk/82) - слайды

#### Dtrace printf debugging for seventh-level wizards
- [http://sartak.org/talks/yapc-asia-2011/dtrace/dtrace.pdf](http://sartak.org/talks/yapc-asia-2011/dtrace/dtrace.pdf) - слайды en/jp

#### AnyEvent, Coro, IO::AIO - mlehmann
- [http://yapcasia.org/2011/talk/71](http://yapcasia.org/2011/talk/71) - слайды и видео

#### Hello Embed Perl! 
- [http://yapcasia.org/2011/talk/43](http://yapcasia.org/2011/talk/43) - слайды

#### Hacking Mac OSX Cocoa API from Perl
О модулях Cocoa::*, блог автора [http://unknownplace.org/memo/](http://unknownplace.org/memo/)

- [http://yapcasia.org/2011/talk/30](http://yapcasia.org/2011/talk/30)

#### Perl Testing Consideration (seen from other languages)
Как я понял, речь о том, что можно еще хорошего позаимствовать из Ruby, чтобы тестирование веб-приложений было проще и приятнее.

- [слайды на slideshare](http://www.slideshare.net/masaki/perl-testing-consideration-seen-from-other-languages)

#### Marc Lehmann о staticperl
100 модулей и Perl в 500 кб (которых должно хватить на всех)
>This script helps you to create single-file perl interpreters or applications, or embedding a perl interpreter in your applications.

- [https://metacpan.org/module/staticperl](https://metacpan.org/module/staticperl)

#### Mote electronic tools in Perl
- [http://yapcasia.org/2011/talk/60](http://yapcasia.org/2011/talk/60)

#### Large-scale environment maniac caching technologies available 
- [http://static.xaicron.dotcloud.com/slide/yapc2011/index.html](http://static.xaicron.dotcloud.com/slide/yapc2011/index.html)

#### "Perl script debugging with gdb" 

к сожалению пока только видео, но тема интересная

- [http://yapcasia.org/2011/talk/61](http://yapcasia.org/2011/talk/61)

#### Hacks image (Image Hacks with Perl)
Про детектинг изображений. На японском, но тоже очень интересная тема.

- [http://yapcasia.org/2011/talk/73](http://yapcasia.org/2011/talk/73) – слайды, видео

#### Watch your log http://nekokak.org/presen/yapcasia2011/ слайды
Про мониторинг и [https://github.com/nekokak/Komainu](https://github.com/nekokak/Komainu)

Автор Nagios Warakan: 

- [https://metacpan.org/author/NEKOKAK](https://metacpan.org/author/NEKOKAK) 
- [https://github.com/nekokak](https://github.com/nekokak)


#### Why high school students use Perl? 
доклад 16-летнего школьника с Хокайдо (самый юный участник).

- [http://akiym.com/slides/20111016-yapcasia2011-why/index.html](http://akiym.com/slides/20111016-yapcasia2011-why/index.html)


#### Web Application Acceleration story 

- [http://ma.la/files/yapcasia2011/](http://ma.la/files/yapcasia2011/) – слайды

#### Hacking with metacpan 
Реклама [metacpan.org](https://metacpan.org)

- [http://tokuhirom.github.com/talks/20111015-yapcasia2011-metacpan/#0](http://tokuhirom.github.com/talks/20111015-yapcasia2011-metacpan/#0) - слайды

#### Whada: Multi-Protocol Authentcation / Authorization Tool 
Рассказ о системе разграничения прав с админкой [https://github.com/tagomoris/whada](https://github.com/tagomoris/whada),
построенной поверх Slapd (OpenLDAP Server).

- [http://yapcasia.org/2011/talk/24](http://yapcasia.org/2011/talk/24) – слайды


#### Evolution of API With Blogging
Узнал о [http://explorer.metacpan.org/](http://explorer.metacpan.org/) и о протоколе [Trackback](http://ru.wikipedia.org/wiki/Trackback).

- [http://yapcasia.org/2011/talk/48](http://yapcasia.org/2011/talk/48) – слайды

#### perlbrew
- [http://yapcasia.org/2011/talk/65](http://yapcasia.org/2011/talk/65) - видео и слайды

#### Carton: CPAN dependencies manager 

- [http://yapcasia.org/2011/talk/91](http://yapcasia.org/2011/talk/91) – слайды

#### A Language for Getting Your Job Done 
Слайды на английском, речь на японском. Доклад совсем не технический, поэтому без расшифровки лектора, по одним слайдам мне было мало чего понятно. )

- [http://www.dan.co.jp/~dankogai/yapcasia2011/jobdone.html](http://www.dan.co.jp/~dankogai/yapcasia2011/jobdone.html)

#### How to Build a Web application is easy to operate
Еще одни слайды на японском в pdf, может быть интересен довольно большой список модулей, о многих узнал впервые

- [http://yapcasia.org/2011/talk/25](http://yapcasia.org/2011/talk/25)
