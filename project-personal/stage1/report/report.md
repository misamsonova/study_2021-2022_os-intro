---
## Front matter
title: "Отчёт по лабораторной работе №4"
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

 Приобрести практические навыки работы с генератором статистических сайтов Hugo, на его основе создать сайт, который может посетить любой пользователь интернета.

# Задание

Размещение на Github pages заготовки для персонального сайта.

- Установить необходимое программное обеспечение.
- Скачать шаблон темы сайта.
- Разместить его на хостинге git.
- Установить параметр для URLs сайта.
- Разместить заготовку сайта на Github pages.

# Выполнение лабораторной работы


1. Скачаем исполняемый файл Hugo для того, чтобы сгенерировать страницу сайта, точнее – архив с репозитория: http://github.com/gohugoio/hugo/releases (рис. [-@fig:001])

![Скачивание исполняемого файла Hugo](images/1.png)

{ #fig:001 width=70% }

2. Создаём папку bin в домашнем каталоге с помощью команды mkdir bin, неё перемещаем файл hugo и переходим по ссылке http://github.com/wowchemy/starter-hugo-academic, чтобы скачать шаблон Hugo Academic Theme индивидуального сайта. Нажимаем кнопку “use this template” и создаём новый репозиторий с именем blog: (рис. [-@fig:002]) и (рис. [-@fig:003])

![Скачивание шаблона Hugo Academic Theme индивидуального сайта](images/2.png)

{ #fig:002 width=70% }

![Создание репозитория с именем blog](images/4.png)

{ #fig:003 width=70% }


3. Далее копируем ссылку на данный репозиторий и переходим в Терминал. С помощью команды git clone копируем содержимое репозитория в каталог blog: (рис. [-@fig:004]) 

![Копирование содержимого репозитория в каталог blog](images/3.png)

{ #fig:004 width=70% }

4. Переходим в каталог blog и проверяем наличие скопированных файлов в каталог blog с помощью команд сd blog/ и ls -l:(рис. [-@fig:005]) 

![Наличие файлов в каталоге blog](images/6.png)

{ #fig:005 width=70% }

5. Далее запускаем наш сайт командой hugo server: (рис. [-@fig:006]) 

![Запуск работы сайта](images/5.png)

{ #fig:006 width=70% }

6. После чего копируем адрес сервера, заходим на сайт и получаем рабочий сайт: (рис. [-@fig:007]) 

![Работа сайта](images/8.png)

{ #fig:007 width=70% }

7. Далее удаляем файл demo.dm, расположенный в content/home/, чтобы убрать зеленый блок с ознакомительной информацией: (рис. [-@fig:008]) и (рис. [-@fig:009])

![Удаление файла demo.dm](images/9.png)

{ #fig:008 width=70% }


![Обновлённый сайт](images/10.png)

{ #fig:009 width=70% }

8. Теперь создадим на github новый репозиторий для того, чтобы сайт могли видеть не только мы, но и другие пользователи интернета. Создаём репозиторий с именем misamsonova.github.io: (рис. [-@fig:010])

![Создание репозитория misamsonova.github.io](images/11.png)

{ #fig:010 width=70% }

9. После чего переходим в Терминал, переходим в домашний каталог, где находится каталог blog, и клонируем репозиторий misamsonova.github.io в домашний каталог с помощью команды git clone --recursive и проверяем наличие данного каталога: (рис. [-@fig:011])

![Копирование файлов с репозитория в каталог blog](images/12.png)

{ #fig:011 width=70% }

10. Переходим в каталог misamsonova.github.io и с помощью команды git checkout –b main мы  создаём новую ветку с именем main :  (рис. [-@fig:012])

![Создание новой ветки репозитория](images/13.png)

{ #fig:012 width=70% }

11. Далее создаём пустой файл README.md с помощью команды touch и с помощью следующий команд обновляем репозиторий с новыми файлами на github. Обнаруживаем, что файл README.md появился на github: (рис. [-@fig:013]) и (рис. [-@fig:014])

![Создание файла README.md и добавление файлов на github](images/14.png)

{ #fig:013 width=70% }

![обновление файлов на github](images/16.png)

{ #fig:014 width=70% }

12. После чего переходим в blog и с помощью команды git submodule add –b main [ссылка на репозиторий] public подключаем репозиторий к папке public, чтобы эффективно генерировать страницы сайта: (рис. [-@fig:015])

![Подключение репозитория к папке public](images/18.png)

{ #fig:015 width=70% }

13. Далее с помощью команды mc переходим в редактор и находим файл .gitignore, в содержимом файла комментируем public/ с помощью символа # и сохраняем. Командой cat .gitignore проверяем изменение содержимого файла: (рис. [-@fig:016]) и (рис. [-@fig:017])

![Изменение файла в редакторе](images/26.png)

{ #fig:016 width=70% }

![Проверка изменения в файле](images/19.png)

{ #fig:017 width=70% }

14. Теперь в связи с изменением одного файла прописываем команду git submodule add –b main [ссылка на репозиторий] public, чтобы изменения вступили в силу: (рис. [-@fig:018])

![Прописание команды для вступления изменений в подключении репозитория к каталогу public](images/20.png)

{ #fig:018 width=70% }

15. Далее вновь запускаем сайт командой hugo: (рис. [-@fig:019])

![Запуск обновлённого сайта](images/23.png)

{ #fig:019 width=70% }

16. Прописываем команду git push origin main, чтобы выполнить отправку изменений конкретной ветки в центральный репозиторий: (рис. [-@fig:020])

![Отправка изменений конкретной ветки в центральный репозиторий](images/25.png)

{ #fig:020 width=70% }

17.  Замечаем, что в каталоге public появились файл: (рис. [-@fig:021])

![Содержание каталога public](images/27.png)

{ #fig:021 width=70% }

18. Возвращаемся в каталог public/. C помощью следующих команд проверяем, что данный каталог подключен к репозиторию misamsonova.github.io, и обновляем файлы в репозитории на github: (рис. [-@fig:022])

![Проверка подключения каталога к репозиторию](images/24.png)

{ #fig:022 width=70% }

19. Обновляем репозиторй и наблюдаем, что появились новые файлы: (рис. [-@fig:023])

![Обновление репозитория](images/28.png)

{ #fig:023 width=70% }

20. Далее вводим в поисковую строку misamsonova.github.io, чтобы проверить, что наш сайт доступен и работает: (рис. [-@fig:024])

![Работа сайта по ссылке misamsonova.github.io](images/29.png)

{ #fig:024 width=70% }


# Вывод

В процессе реализации 1-ого этапа мы приобрели практические навыки работы с генератором статистических сайтов Hugo, на его основе создали свой сайт, который может посетить любой пользователь интернета.
