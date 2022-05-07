---
## Front matter
title: "Отчёт по 2 этапу реализации проекта"
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

Приобрести практические навыки размещения информации о себе и выкладывания постов на собственном сайте путем редактирования файлов в каталогах, создания новых файлов и каталогов и обновления через Терминал файлов.

# Задание

Добавить к сайту данные о себе:

- Разместить фотографию владельца сайта.
- Разместить краткое описание владельца сайта (Biography).
- Добавить информацию об интересах (Interests).
- Добавить информацию об образовании (Education).
- Сделать пост по прошедшей неделе.
- Добавить пост на тему по выбору:
  - Управление версиями. Git.
  - Непрерывная интеграция и непрерывное развертывание (CI/CD).

# Реализация 2 этапа проекта

1. Для начала запустим созданный сайт: (рис. [-@fig:001])

![Запуск работы сайта](images/0.png)

{ #fig:001 width=70% }

2. Изменим информацию о себе, отыскав файл _index.md в каталоге *~/blog/content/authors/admin* и внеся в него основные сведения (образование, имя и фамилия, сайт университета, интересы и пр.):(рис. [-@fig:002]) и (рис. [-@fig:003])

![Изменение информации о себе](images/1.png)

{ #fig:002 width=70% }

![Изменение информации о себе](images/2.png)

{ #fig:003 width=70% }

3. Меняем фотографию на странице, загрузив фотографию в каталог *~/blog/content/authors/admin* и переименовав в avatar.jpg: (рис. [-@fig:004])

![Изменение фотографии на сайте](images/3.png)

{ #fig:004 width=70% }

4. Открываем сайт, чтобы удостовериться, что изменения применены: (рис. [-@fig:005])

![Изменение информации на сайте](images/4.png)

{ #fig:005 width=70% }

5. Далее мы переходим в каталог *~/blog/content/post*, создаём новые каталоги "my last week" и "About git" и копируем в них файл _index.md: (рис. [-@fig:006])

![Создание новых папок](images/5.png)

{ #fig:006 width=70% }

6. Теперь переходим в каталог "my last week" и в файле _index.md добавляем информацию о прошедшей неделе. Также добавляем в данный каталог картинку: (рис. [-@fig:007])

![Редактирование информации в файле](images/6.png)

{ #fig:007 width=70% }

7. После этого переходим в каталог "About git" и в файле _index.md добавляем информацию об управлении версиями git, также добавляем в данный каталог картинку: (рис. [-@fig:008]), (рис. [-@fig:009]) и (рис. [-@fig:010])

![Редактирование информации в файле](images/8.png)

{ #fig:008 width=70% }

![Добавлении картинки](images/9.png)

{ #fig:009 width=70% }

![Добавлении картинки](images/7.png)

{ #fig:010 width=70% }

8. Открываем сайт, чтобы удостовериться, что изменения применены: (рис. [-@fig:011])

![Добавление постов на сайте](images/10.png)

{ #fig:011 width=70% }

9. Также замечаем, что наши изменения фиксируются в Терминале: (рис. [-@fig:012])

![Вывод об изменениях сайта в Терминале](images/11.png)

{ #fig:012 width=70% }

10. Теперь следующими командами мы обновляем файлы на github и запускаем сервер для просмотра другими пользователями сайта с уже изменённой информацией:(рис. [-@fig:013]),(рис. [-@fig:014]),(рис. [-@fig:015])

![Ввод команд для обновления файлов на github](images/12.png)

{ #fig:013 width=70% }

![Запуск сервера и ввод команд для обновления файлов на github](images/13.png)

{ #fig:014 width=70% }

![Загрузка обновлённых файлов на github](images/14.png)

{ #fig:015 width=70% }

11.  Открываем github, чтобы удостовериться, что изменения применены: (рис. [-@fig:016])

![Обновлённые папки на github](images/15.png)

{ #fig:016 width=70% }

12. Запускаем сайт misamsonova.github.io через терминал командой hugo и просматриваем посты, убеждаемся, что всё имеется:(рис. [-@fig:017]),(рис. [-@fig:018]), (рис. [-@fig:019]),(рис. [-@fig:020])

![Просмотр поста "my last week" на сайте](images/16.png)

{ #fig:017 width=70% }

![Просмотр поста "Version control.Git." на сайте](images/17.png)

{ #fig:017 width=70% }

![Просмотр  поста "Version control.Git." на сайте](images/18.png)

{ #fig:017 width=70% }

![Просмотр поста "Version control.Git." на сайте](images/19.png)

{ #fig:017 width=70% }


# Вывод

В процессе реализации 2-ого этапа мы приобрели практические навыки размещения информации о себе и выкладывания постов на собственном сайте путем редактирования файлов в каталогах, создания новых файлов и каталогов и обновления через Терминал файлов.