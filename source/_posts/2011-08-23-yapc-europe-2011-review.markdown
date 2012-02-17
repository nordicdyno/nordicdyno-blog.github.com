---
layout: post
title: "Обзор YAPC::Europe 2011"
date: 2011-08-23 17:31
comments: true
categories: [Perl, YAPC, Review]
---


На прошлой неделе я посетил Perl-конференцию [YAPC::Europe 2011 “Modern Perl”](http://yapceurope.lv/ye2011/), которая проходила в Риге. 
Помимо того, что мне удалось сфотографироваться с Ларри Уоллом и получить от него и Дэмиана Конвея автографы, потусить с гиками со всего мира и разжиться сувенирными футболками, я исправно посещал презентации в течении тех трех дней, что шла конференция, и даже немножечко пытался конспектировать то что слышал. )
Ниже список тех выступлений, на которых удалось побывать, с моими кратким комментариями. 

<!-- more -->

## 1-й день

### Larry Wall's keynote
Ларри выступил в своей привычной  роли идеолога и философа Perl-коммьюнити, взяв темой своих рассуждений (размышлений)  "Modern perl". Мне было очень интересно.)

* [http://yapceurope.lv/ye2011/talk/3531](http://yapceurope.lv/ye2011/talk/3531)

### How not to screw up your business application
Carl Mäsak рассказывал о [CQRS](http://martinfowler.com/bliki/CQRS.html) на примере приложения, обслуживающего пассажиропоток в аэропорту

* [http://yapceurope.lv/ye2011/talk/3517](http://yapceurope.lv/ye2011/talk/3517)

### Oriental Perl for Enterprise

Юсуке Кавасаки о использовании Perl в японском энтерпрайзе, на примере своего работодателя [RWS](http://www.rws.com/) (японский медиа-гигант)

* [http://yapceurope.lv/ye2011/talk/3472](http://yapceurope.lv/ye2011/talk/3472)

### Making data dance

Carl Mäsak о использовании Perl 5/6 для решения комбинаторных задач. Я так понял, что в качестве визуализатора и прототипирования алгоритма (по сути обвязка для C),

- [http://yapceurope.lv/ye2011/talk/3518](http://yapceurope.lv/ye2011/talk/3518)

### Replacing Relational DB with Redis: a Case Study

Повестование о том, как хранилище DHCP-сервиса перевели из постгреса в редиску. Если честно, я не дослушал, т.к. было скучно.

- [http://yapceurope.lv/ye2011/talk/3482](http://yapceurope.lv/ye2011/talk/3482)

### Tapper test scheduling

Инженер из AMD о внутреннем тестовом фреймворке на Perl, который они выложили в opensource [https://github.com/amd](https://github.com/amd)

- [http://yapceurope.lv/ye2011/talk/3430](http://yapceurope.lv/ye2011/talk/3430)

### Smoking The Onion - Tales of CPAN Testers

Рассказ о [cpantesters.org](http://www.cpantesters.org/)
Я лично ожидал, что будет интереснее. Какие нибудь истории из жизни тестеров, например.

- [http://yapceurope.lv/ye2011/talk/3547](http://yapceurope.lv/ye2011/talk/3547)
 

## Второй день

### Damian Conway (damian) - (Re)Developing in Perl 6

Автор множества модулей http://search.cpan.org/~dconway/ и PhD из Мельбурна о том, как круто будет писать на Perl6 )

- [http://yapceurope.lv/ye2011/talk/3532](http://yapceurope.lv/ye2011/talk/3532)

### Zefram - bending semantics with 5.14

Этот доклад я не дослушал, т.к. не понял какую проблему хотел решить автор, да и код на слайдах мне не был хорошо виден, а во круг его объяснения строился рассказ

- [http://yapceurope.lv/ye2011/talk/3325](http://yapceurope.lv/ye2011/talk/3325)
 
### Steffen Schwigon (renormalist) - Benchmark::Perl::Formance for the masses
Немец пообещал веб-сервис для бенчмаркинга на основе tapper ("через 2 недели")

- [http://yapceurope.lv/ye2011/talk/3467](http://yapceurope.lv/ye2011/talk/3467)

### Andrew Solomon - Dancing into Web Development

Автор предложил на коленке собрать очень простой сайт на Dancer, мне это не показалось интересным и я сбежал на параллельный доклад

- [http://yapceurope.lv/ye2011/talk/3591](http://yapceurope.lv/ye2011/talk/3591)


### Maciej Czekay (Bruno) - Perl Jam: processing MIDI events in realtime
 Интересная демонстрация модуля для фильтрации MIDI-событий (только для Линукс). По сути игрушка для экспериментов с синтезируемой компьютером музыкой (for free). 
 А вообще приятно и интересно наблюдать таких увлекающихся людей как автор (в данном случае музыкой и Perl)

- [http://yapceurope.lv/ye2011/talk/3536](http://yapceurope.lv/ye2011/talk/3536)

### Reini Urban (rurban) - use types

Мантейнер perl и cygwin о возможных нововведениях в perl 5.16. О реализации оптимизаций по скорости и памяти на основе указания программистом типов переменных в коде (опционально). Также о планах добавления возможности выбора программистом механизма хэширования и поддержки алгоритма "Perfect hash" (O(1) BDZ algorithm)

- [http://yapceurope.lv/ye2011/talk/3288](http://yapceurope.lv/ye2011/talk/3288)
 

### The Perl Foundation: Year in Review

Президент TPF о пожертвованиях, работе и успехах/неудачах фонда. Интересно с точки зрения того как живет и устроен Open Source.

- [http://yapceurope.lv/ye2011/talk/3650](http://yapceurope.lv/ye2011/talk/3650)

### Plack basics - website best practices

О том, что такое PSGI и Plack и о инфраструктуре вокруг Plack (Plack::App:: Plack::Middleware).

- [http://yapceurope.lv/ye2011/talk/3380](http://yapceurope.lv/ye2011/talk/3380)

### Mark Keating (mdk) - Adventures in Marketing

В основном, автор с говорящим именем (псевдонимом?), говорил о пользе PR Perl и об успехах за последние несколько лет в этом направлении.

- [http://yapceurope.lv/ye2011/talk/3364](http://yapceurope.lv/ye2011/talk/3364)


## День третий

### Perl 5.16 and Beyond
Очень интересный доклад, но застал только концовку, из-за того что тупо проспал. :(
Основной лидер и координатор разработки perl5 Jesse Vincent о успехах в разработке Perl5 и какие есть планы на будущее.

- [http://yapceurope.lv/ye2011/talk/3291](http://yapceurope.lv/ye2011/talk/3291)
- [http://www.slideshare.net/obrajesse/perl-516-and-beyond](http://www.slideshare.net/obrajesse/perl-516-and-beyond)

### Modern Perl - getting there from here

Англичанин рассказал как они распиливали свою легаси систему (что-то B2B-шное, связанное с налогообложением) и постепенно по кусочкам переписывали. В результате получили новую-кленовую с лучшим интерфейсом, оттестированную. документированную и с модерновым-перлом унутре.

- [http://yapceurope.lv/ye2011/talk/3652](http://yapceurope.lv/ye2011/talk/3652)

### Introduction to the Dancer web application framework

Yet Another презентация о фреймворке Dancer. Я ничего нового не узнал, но вообще хороший старт для интересующихся, но еще не "пощупавших".

- [http://yapceurope.lv/ye2011/talk/3543](http://yapceurope.lv/ye2011/talk/3543)

### Running legacy mod_perl with Plack

Peter Makholm из Копенгагена рассказал, как он не любит разрабатывать под mod_perl.
Настолько, что написал свою обертку для запуска mod_perl приложений под plack-ом (использует только для девелопмента). Полученный профит – тесты, няшные миддлваре (StackTrace) и удобство в разработке. В продакшене обертку они не используют.

- [http://yapceurope.lv/ye2011/talk/3432](http://yapceurope.lv/ye2011/talk/3432)

### Yusuke Kawasaki (kawanet) - Hack For Japan

После недавнего землятресения в Японии, японские хакеры помогали тем, что умеют хорошо, а именно писали код. Рассказ о том, как были организованы хакатоны, какие полезные сервисы и приложения были созданы. Особенно интересно про самодельные счетчики Гейгера (они не продаются в японских магазинах, если что). 

- [http://yapceurope.lv/ye2011/talk/3471](http://yapceurope.lv/ye2011/talk/3471)

### Lars Dɪᴇᴄᴋᴏᴡ (迪拉斯) - Encryption on the Web for everyone

Это единственный доклад, где мне казалось, что я сейчас клюну носом и уроню ноутбук с колен (может только поэтому и не заснул).
Не то что бы тема такая не интересная (интересная и важная!), но вот докладчик был как настоящий кот-баюн. )
В основном Ларс рассказывал о том, как распилили на модули LWP 6-й версии, и какая непростая штука ssl, во многом из-за бардака с сертификатами, как намучались с OpenSSL. Сейчас SSL из LWP выпилен в отдельный модуль LWP::Protocol::https и еще существует модуль Mozilla::CA, в котором храняться копии корневых сертификатов, что типа некрасиво. но зато работает (в curl сделано также).

- [http://yapceurope.lv/ye2011/talk/3628](http://yapceurope.lv/ye2011/talk/3628)

ссылки по теме:

- Firesheep ([http://www.rb.ru/topstory/science/2010/10/26/185603.html](http://www.rb.ru/topstory/science/2010/10/26/185603.html))
- Monkeysphere ([http://web.monkeysphere.info/why/#index1h2](http://web.monkeysphere.info/why/#index1h2))
- [http://vttynotes.blogspot.com/2010/12/man-in-middle-fun-with-perl-lwp.html](http://vttynotes.blogspot.com/2010/12/man-in-middle-fun-with-perl-lwp.html)
- intermediate certificates [http://vttynotes.blogspot.com/2011/03/quick-note-on-lwp-and-perl-security-cve.html](http://vttynotes.blogspot.com/2011/03/quick-note-on-lwp-and-perl-security-cve.html)

### Abigail - The Business Aware Programmer

Дядька из booking.com нудно рассказывал о интересах бизнеса ($$$$), и раскрыл Секрет Полишинеля, о том, что то, что программисты считают ценностями (рефакторинг, тесты, правильная архитектура), могут не являться таковыми для бизнеса (если в итоге не приносят $$$). Вобщем, непонятно зачем он просил не записывать свой доклад, и чего такого секретного в итоге рассказал.

Мое резюме такое, что доклад годный в плане прочистки некоторых программистских мозгов. Да, думать как бизнесмен разработчику обычно не нужно, но понимать скучных дядек в костюмах надо и полезно, все-таки они в конечном итоге занимаются возгонкой денег из кода :)

- [http://yapceurope.lv/ye2011/talk/3510](http://yapceurope.lv/ye2011/talk/3510)

### Matt S Trout (mst) - State of the Velociraptor

Экспрессивная речь (как обычно) известного разработчика и пропагандиста Perl Мэта Траута. Правда матерился он меньше обычного и вообще общий настрой у доклада был позитивный. Мэт рассказал о том, как обратить в свою пользу особенности поведения персонажей в интернете, которых он классифицировал как assholes, idiots, whiners, trolls. При этом из зала в него летели плюшевые ктулху, одним из которых он потом перестреливался с Ларри Уоллом. А я утащил потом одного домой на память. )

- [http://yapceurope.lv/ye2011/talk/3316](http://yapceurope.lv/ye2011/talk/3316)

### мой хит-парад докладов

1. Larry Wall's keynote
2. Yusuke Kawasaki (kawanet) - Hack For Japan
3. The Perl Foundation: Year in Review
4. Damian Conway (damian) - (Re)Developing in Perl 6
5. Reini Urban (rurban) - use types
6. Perl 5.16 and Beyond
7. Matt S Trout (mst) - State of the Velociraptor
