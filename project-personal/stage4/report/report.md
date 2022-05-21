---
## Front matter
title: "Отчёт по 4 этапу реализации проекта"
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

Приобрести практические навыки размещения информации о себе (контакты/ссылки сайтов, где можно найти меня) и выкладывания постов на собственном сайте путем редактирования файлов в каталогах, создания новых файлов и каталогов и обновления через Терминал файлов.

# Задание

Добавить к сайту ссылки на научные и библиометрические ресурсы:

1. Зарегистрироваться на соответствующих ресурсах и разместить на них ссылки на сайте:
- eLibrary : https://elibrary.ru/;
- Google Scholar : https://scholar.google.com/;
- ORCID : https://orcid.org/;
- Mendeley : https://www.mendeley.com/;
- ResearchGate : https://www.researchgate.net/;
- Academia.edu : https://www.academia.edu/;
- arXiv : https://arxiv.org/;
- github : https://github.com/.
2. Сделать пост по прошедшей неделе.
3. Добавить пост на тему по выбору:
- Оформление отчёта.
- Создание презентаций.
- Работа с библиографией.

# Реализация 3-его этапа индивидуального проекта

1. Для начала запустим наш сайт: (рис. -@fig:001)

![Запуск работы сайта](image/1.png)

{ #fig:001 width=70% }

- Зарегистрируемся на следующих сайтах (по заданию): (рис. -@fig:002, -@fig:003, -@fig:004, -@fig:005, -@fig:006, -@fig:007, -@fig:008, -@fig:009, -@fig:010, -@fig:011, -@fig:012, -@fig:013, -@fig:014, -@fig:015)

![Список сайтов, на которых надо зарегистрироваться](image/2.png)

{ #fig:002 width=70% }

![Регистрация на сайте eLibrary](image/3.png)

{ #fig:003 width=70% }

![Регистрация на сайте eLibrary](image/4.png)

{ #fig:004 width=70% }

![Регистрация на сайте Orcid](image/5.png)

{ #fig:005 width=70% }

![Регистрация на сайте Orcid](image/6.png)

{ #fig:006 width=70% }

![Регистрация на сайте Orcid](image/7.png)

{ #fig:007 width=70% }

![Регистрация на сайте Mendeley](image/8.png)

{ #fig:008 width=70% }

![Регистрация на сайте Mendeley](image/9.png)

{ #fig:009 width=70% }

![Регистрация на сайте ResearchGate](image/10.png)

{ #fig:010 width=70% }

![Регистрация на сайте ResearchGate](image/11.png)

{ #fig:011 width=70% }

![Регистрация на сайте Academia](image/12.png)

{ #fig:012 width=70% }

![Регистрация на сайте Academia](image/13.png)

{ #fig:013 width=70% }

![Регистрация на сайте Arxiv](image/14.png)

{ #fig:014 width=70% }

![Регистрация на сайте Arxiv](image/15.png)

{ #fig:015 width=70% }

- Добавим эти ссылки на наш сайт, отыскав файл _index.md в каталоге *~/blog/content/authors/admin*, внеся в него ссылки и вставив названия подходящих иконок со следующего сайта: (рис. -@fig:016, -@fig:017)

![Редактирование файла index.md](image/16.png){#fig:016 width=70%}

![Редактирование файла index.md](image/18.png){#fig:017 width=70%}

- После этого сохраняем файл и закрываем его. Переходим на сайт, чтобы убедиться, что сайт учёл изменения: (рис. -@fig:018)

![Обновлённый сайт](image/17.png)

{ #fig:018 width=70% }


2.  Далее мы переходим в каталог *~/blog/content/post*, создаём новые каталоги "Last week 21.05.22" и "Оформление отчёта" и копируем в них файл _index.md из имеющихся каталогов (прошлых постов): (рис. -@fig:019)

![Создание каталогов](image/21.png)

{ #fig:019 width=70% }

- Теперь переходим в каталог "Last week 21.05.22" и в файле _index.md добавляем информацию о прошедшей неделе. Также добавляем в данный каталог скачанную картинку: (рис. -@fig:020, -@fig:021)

![Написание поста](image/19.png)

{ #fig:020 width=70% }

![Добавление картинки](image/20.png)

{ #fig:021 width=70% }

3. После этого переходим в каталог "Оформление отчёта" и в файле _index.md пишем пост об оформлении отчёта в Markdown, также добавляем в данный каталог картинку: (рис. -@fig:022, рис. -@fig:023 и рис. -@fig:024)

![Написание поста](image/22.png)

{ #fig:022 width=70% }

![Написание поста](image/23.png)

{ #fig:023 width=70% }

![Добавление картинки](image/24.png)

{ #fig:024 width=70% }

4. Теперь следующими командами в Терминале запускаем наш сайт для всех пользователей интернета, обновляем загружаем новые каталоги и файлы в репозиторий blog на github и, перейдя в каталог public, загружаем также все каталоги и файлы в репозиторий misamsonova.github.io на github для того, чтобы обновился сайт, который могут посетить все пользователи интернета:(рис. -@fig:025, -@fig:026, -@fig:027)

![Запуск сервера и загрузка файлов командами](image/25.png)

{ #fig:025 width=70% }

![Загрузка файлов](image/26.png)

{ #fig:026 width=70% }

![Обновление репозиторий на github](image/27.png)

{ #fig:027 width=70% }

- Наконец, перейдём на сайт misamsonova.github.io, который доступен всем пользователям интернета, и проверим, обновился ли сайт. Как мы замечаем, всё появилось:(рис. -@fig:028, -@fig:029, -@fig:030, -@fig:031, -@fig:032)

![Обновлённый сайт](image/28.png)

{ #fig:028 width=70% }

![Наличие новых постов](image/29.png)

{ #fig:029 width=70% }

![Содержание новых постов](image/30.png)

{ #fig:030 width=70% }

![Содержание новых постов](image/31.png)

{ #fig:031 width=70% }

![Содержание новых постов](image/32.png)

{ #fig:032 width=70% }

![Содержание новых постов](image/33.png)

{ #fig:033 width=70% }

# Вывод

В процессе реализации 4-ого этапа мы приобрели практические навыки размещения информации о себе (контакты/ссылки сайтов, где можно найти меня) и выкладывания постов на собственном сайте путем редактирования файлов в каталогах, создания новых файлов и каталогов и обновления через Терминал файлов.
