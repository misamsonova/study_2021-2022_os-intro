---
## Front matter
title: "Отчёт по лабораторной работе №3"
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

Научиться оформлять отчёты с помощью легковесного языка разметки Markdown.

# Задание

Составить отчёт по выполнению лабораторной работы №2.

# Теоретическое введение

## Базовые сведения о Markdown
Чтобы создать заголовок, используйте знак ( # ) и уберите кавычки, например:
"# This is heading 1"
"## This is heading 2"
"### This is heading 3"
"#### This is heading 4"

Чтобы задать для текста полужирное начертание, заключите его в двойные звездочки и уберите пробелы между символами и звездочками:
This text is ** bold **.

Чтобы задать для текста курсивное начертание, заключите его в одинарные звездочки и уберите пробелы между символами и звездочками:
This text is * italic *.

Чтобы задать для текста полужирное и курсивное начертание, заключите его в тройные
звездочки и уберите пробелы между символами и звездочками:
1 This is text is both *** bold and italic ***.

Блоки цитирования создаются с помощью символа > (уберите кавычки):
 
">" The drought had lasted now for ten million years, and the reign of
the terrible lizards had long since ended. Here on the Equator, in
the continent which would one day be known as Africa, the battle
for existence had reached a new climax of ferocity, and the victor
was not yet in sight. In this barren and desiccated land, only the
small or the swift or the fierce could flourish, or even hope to
survive.

Неупорядоченный (маркированный) список можно отформатировать с помощью звездочек или тире (поставьте пробел между тире/звездой и заголовком):

-List item 1

-List item 2

-List item 3
 
# Выполнение лабораторной работы

1. Указание данных о работе (название работы, название дисциплины, по которой выполняется работа, ФИО выполняющего): (рис. [-@fig:001])

![Указание основной информации о выполнении отчёта](images/1.png)
{ #fig:001 width=70% }

2. Указание цели лабораторной работы №2 с помощью заглавия, начинающегося с # [Название_заглавия]: (рис. [-@fig:002])

![Указание цели лабораторной работы](images/2.png)
{ #fig:002 width=70% }

3. Указание заданий, которые требовалось выполнить в лабораторной работе №2, с помощью заглавия, начинающегося с # [Название_заглавия], и тире, которые помогают перечислить определённые пункты заданий: (рис. [-@fig:003])

![Указание заданий лабораторной работы](images/3.png)

{ #fig:003 width=70% }

4. Указание теоретического введения лабораторной работы №2 с помощью заглавия, начинающегося с # [Название_заглавия]:(рис. [-@fig:004])

![Указание теоретического введения лабораторной работы](images/4.png)

{ #fig:004 width=70% }

5. Прописывание хода выполнения лабораторной работы №2 с помощью заглавия, начинающегося с # [Название_заглавия], нумерации определённой цифрой и точкой и добавления скринов с помощью данного шаблона без кавычек: (рис. [-@fig:005])

**Шаблон**:
**[ "(рис. [-@fig:003])![Указание заданий лабораторной работы]"(название_папки/номер_скрина.png)"{ #fig:003 width=70% }"]**

![Прописывание хода выполнения лабораторной работы](images/5.png)

{ #fig:005 width=70% }

6. Указание вывода лабораторной работы №2 с помощью заглавия, начинающегося с # [Название_заглавия]: (рис. [-@fig:006])

![Указание вывода лабораторной работы](images/6.png)

{ #fig:006 width=70% }



# Вывод
В процессе выполнения лабораторной работы №3 мы научились оформлять отчёты с помощью легковесного языка разметки Markdown.


