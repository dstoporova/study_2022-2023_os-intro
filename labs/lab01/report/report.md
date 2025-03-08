---
## Front matter
title: "Лабораторная работа №1"
subtitle: "По операционным системам"
author: "Топорова Дарья Сергеевна НММбд-03-24"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

1. Установить и настроить виртуальную машину
2. Скачать все необходимые файлы и также настроить для дальнейшей работы
# Выполнение лабораторной работы

После скачивания Oracle VirtualBox необходимо настроить виртуальную машину в соответствии с требованиями (рис. [-@fig:001]).

![Настроенная виртуальная машина](image/p1.jpg){#fig:001 width=70%}

Для того чтобы установить и настроить необходимые файлы, нужно перейти в режим супер-пользователя(рис. [-@fig:002]).

![переключение на роль супер-пользователя](image/p2.jpg){#fig:002 width=70%}

Установим необходимые средства разработки(рис. [-@fig:003]).

![установка средств разработки](image/p3.jpg){#fig:003 width=70%}

Также требуется обновить все пакеты(рис. [-@fig:004]).

![обновление](image/p4.jpg){#fig:004 width=70%}

Установим программы для удобства работы в консоли(рис. [-@fig:005]).

![программы для консоли](image/p5.jpg){#fig:005 width=70%}

После установки программного обеспечения для автоматический обновлений установим таймер(рис. [-@fig:006]).

![таймер для обновлений](image/p6.jpg){#fig:006 width=70%}

Так как в данном курсе не будет рассматриваться работа с системой безопасности SELinux, то нам надо отключить её(рис. [-@fig:007]).

![отключение SELinux](image/p7.jpg){#fig:007 width=70%}

После всех изменений необходимо перезагрузить систему(рис. [-@fig:008]).

![перезагрузка виртуальной машины](image/p8.jpg){#fig:008 width=70%}

Создаём конфигурационный файл(рис. [-@fig:009]).

![конфигурационный файл](image/p9.jpg){#fig:009 width=70%}

Отредактируем конфигурационный файл(рис. [-@fig:010]).

![изменение конфигурационного файл](image/p10.jpg){#fig:010 width=70%}

Изменим имя пользователя, название хоста и пароль(рис. [-@fig:011]).

![изменение имени пользователя, хоста и пароля](image/p11.jpg){#fig:011 width=70%}

Установим pandoc  для работы с языком разметки Markdown(рис. [-@fig:012]).

![Установка pandoc](image/p12.jpg){#fig:012 width=70%}

Установим также pandoc-crossref (рис. [-@fig:013]) (рис. [-@fig:014])(рис. [-@fig:015]).

![Установка pandoc-crossref 1](image/p13.jpg){#fig:013 width=70%}
![Установка pandoc-crossref 2](image/p14.jpg){#fig:014 width=70%}
![Установка pandoc-crossref 3](image/p15.jpg){#fig:015 width=70%}

Необходимо установить дистрибутив TeXlive(рис. [-@fig:016]).

![Установка дистрибутива TeXlive](image/p16.jpg){#fig:016 width=70%}

# Домашнее задание 

С помощью команды dmesg | grep -i "то, что ищем", найдём версию ядра Linux, частоту процессора, модель процессора(рис. [-@fig:017]).

![поиск с помощью команды grep](image/p17.jpg){#fig:017 width=70%}

# Выводы

После выполнения данной лабораторной работы я приобрела практические навыки по установке операционной системы на виртуальную машину и настройки минимально необходимых для дальнейшей работы сервисов.


