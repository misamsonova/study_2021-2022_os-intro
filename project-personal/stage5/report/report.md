---
## Front matter
title: "Отчёт по 5 этапу реализации проекта"
subtitle: "Операционные системы"
author: "Самсонова Мария Ильинична"
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
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
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

Приобретение практических навыков размещения информации о себе (проект) и выкладывания постов на собственном сайте путем редактирования файлов в каталогах, создания новых файлов и каталогов и обновления через Терминал файлов.

# Задание

Добавить с сайту все остальные элементы:

- Сделать записи для персональных проектов.
- Сделать пост по прошедшей неделе.
- Добавить пост на тему "Языки научного программирования".

# Реализация 5-его этапа индивидуального проекта

1. Для начала запустим наш сайт: (рис. -@fig:001)

![Запуск работы сайта](image/1.png){ #fig:001 width=70% }

2. Далее мы переходим в каталог *~/blog/content/project/example*,редактируем файл _index.md, в котором пишем о своём проекте " Python или Java. Что лучше выбрать для изучения?". Также добавляем в данный каталог скачанную картинку : (рис. -@fig:002, -@fig:003, -@fig:004, -@fig:005)

![Переход в нужный каталог](image/2.png){ #fig:002 width=70% }

![Написание проекта](image/3.png){ #fig:003 width=70% }

![Написание проекта](image/4.png){ #fig:004 width=70% }

![Добавление картинки](image/5.png){ #fig:005 width=70% }

3. Теперь переходим в каталог  *~/blog/content/post*, создаём каталог "Last week 28.05.22" и в файле _index.md добавляем информацию о прошедшей неделе. Также добавляем в данный каталог скачанную картинку: (рис. -@fig:006, -@fig:007, -@fig:008)

![Переход в нужный каталог](image/6.png){ #fig:006 width=70% }

![Написание поста](image/7.png){ #fig:007 width=70% }

![Добавление картинки](image/8.png){ #fig:008 width=70% }

- После этого создаём каталог "Языки научного программирования" и в файле _index.md добавляем информацию о них. Также добавляем в данный каталог скачанную картинку: (рис. -@fig:009, -@fig:010, -@fig:011,-@fig:012)

![Добавление картинки](image/9.png){ #fig:009 width=70% }

![Написание поста](image/10.png){ #fig:010 width=70% }

![Написание поста](image/11.png){ #fig:011 width=70% }

![Написание поста](image/12.png){ #fig:012 width=70% }

4. Теперь перейдем на сайт и проверим, учтены ли изменения. Как мы видим появился проект и добавились новые посты:(рис. -@fig:013, -@fig:014)
 
![Проект](image/13.png){ #fig:013 width=70% }

![Посты](image/14.png){ #fig:014 width=70% }

5. Теперь следующими командами в Терминале запускаем наш сайт для всех пользователей интернета, обновляем загружаем новые каталоги и файлы в репозиторий blog на github и, перейдя в каталог public, загружаем также все каталоги и файлы в репозиторий misamsonova.github.io на github для того, чтобы обновился сайт, который могут посетить все пользователи интернета:(рис. -@fig:015, -@fig:016, -@fig:017)

![Запуск сервера и загрузка файлов командами](image/15.png){ #fig:015 width=70% }

![Загрузка файлов](image/16.png){ #fig:016 width=70% }

![Обновление репозиторий на github](image/17.png){ #fig:017 width=70% }

- Наконец, перейдём на сайт misamsonova.github.io, который доступен всем пользователям интернета, и проверим, обновился ли сайт. Как мы замечаем, всё появилось:(рис. -@fig:018, -@fig:019, -@fig:020, -@fig:021, -@fig:022)

![Наличие новых постов](image/18.png){ #fig:018 width=70% }

![Содержание новых постов](image/19.png){ #fig:019 width=70% }

![Содержание новых постов](image/20.png){ #fig:020 width=70% }

![Появление на обновлённом сайте проекта](image/21.png){ #fig:021 width=70% }

![Содержание проекта](image/22.png){ #fig:022 width=70% }

# Вывод

В процессе реализации 5-ого этапа мы приобрели практические навыки размещения информации о себе (проект) и выкладывания постов на собственном сайте путем редактирования файлов в каталогах, создания новых файлов и каталогов и обновления через Терминал файлов.

