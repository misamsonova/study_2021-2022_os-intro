---
## Front matter
title: "Отчёт по лабораторной работе №7"
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

Освоение основных возможностей командной оболочки Midnight Commander. Приобретение навыков практической работы по просмотру каталогов и файлов; манипуляций с ними.

# Задание

**Задание по mc:**

1. Изучите информацию о mc, вызвав в командной строке man mc.
2. Запустите из командной строки mc, изучите его структуру и меню.
3. Выполните несколько операций в mc, используя управляющие клавиши (операции
с панелями; выделение/отмена выделения файлов, копирование/перемещение файлов, получение информации о размере и правах доступа на файлы и/или каталоги
и т.п.)
4. Выполните основные команды меню левой (или правой) панели. Оцените степень
подробности вывода информации о файлах.
5. Используя возможности подменю Файл , выполните:
- просмотр содержимого текстового файла;
- редактирование содержимого текстового файла (без сохранения результатов редактирования);
- создание каталога;
- копирование в файлов в созданный каталог.
6. С помощью соответствующих средств подменю Команда осуществите:
- поиск в файловой системе файла с заданными условиями (например, файла с расширением .c или .cpp, содержащего строку main);
- выбор и повторение одной из предыдущих команд;
- переход в домашний каталог;
- анализ файла меню и файла расширений.
7. Вызовите подменю Настройки . Освойте операции, определяющие структуру экрана mc (Full screen, Double Width, Show Hidden Files и т.д.)

**Задание по встроенному редактору mc:**
1. Создайте текстовой файл text.txt.
2. Откройте этот файл с помощью встроенного в mc редактора.
3. Вставьте в открытый файл небольшой фрагмент текста, скопированный из любого
другого файла или Интернета.
4. Проделайте с текстом следующие манипуляции, используя горячие клавиши:
- Удалите строку текста.
- Выделите фрагмент текста и скопируйте его на новую строку.
- Выделите фрагмент текста и перенесите его на новую строку.
- Сохраните файл.
- Отмените последнее действие.
- Перейдите в конец файла (нажав комбинацию клавиш) и напишите некоторый
текст.
- Перейдите в начало файла (нажав комбинацию клавиш) и напишите некоторый
текст.
- Сохраните и закройте файл.
5. Откройте файл с исходным текстом на некотором языке программирования (например C или Java)
6. Используя меню редактора, включите подсветку синтаксиса, если она не включена,
или выключите, если она включена.


# Выполнение лабораторной работы

1. Для начала изучили информацию о mc, вызвав в командной строке «man mc» ( рис. -@fig:001 , -@fig:002). 
Midnight Commander (или mc) − псевдографическая командная оболочка для UNIX/Linux систем. Для запуска mc необходимо в командной строке набрать «mc» и нажать«enter».

![Работа с консолью](image/1.png)

{#fig:001 width=70%}

![Справка по команде mc](image/2.png)

{#fig:002 width=70%}

2. Далее запустили из командной строки mc и изучили его структуру и меню (рис. -@fig:003 , -@fig:004 , -@fig:005 , -@fig:006 , -@fig:007 , -@fig:008 , -@fig:009 , -@fig:010 , -@fig:011 ).
Заметили, что в стандартном состояние окно редактора состоит из двух панелей (рис. -@fig:004 ).
Верхнее меню содержит меню «Левая панель», «Файл», «Команда», «Настройки», «Правая панель» (Рисунки -@fig:005 , -@fig:006 , -@fig:007 , -@fig:008 , -@fig:009 ). Нажав клавишу «F2», можно открыть «Меню пользователя» (Скриншот -@fig:010). Нажав клавишу «F1», можно открыть «Помощь» (рис. -@fig:011).

![Вызов команда mc](image/3.png)

{ #fig:003 width=70% }

![Команда mc](image/4.png)

{ #fig:004 width=70% }

![Левая панель в mc](image/5.png)

{ #fig:005 width=70% }

![Файл в mc](image/6.png)

{ #fig:006 width=70% }

![Команда в mc](image/7.png)

{ #fig:007 width=70% }

![Настройки в mc](image/8.png)

{ #fig:008 width=70% }

![Правая панель в mc](image/9.png)

{ #fig:009 width=70% }

![Меню пользователя в mc](image/10.png)

{ #fig:010 width=70% }

![Помощь в mc](image/11.png)

{ #fig:011 width=70% }

3. После этого выполнили операции в mc, используя управляющие клавиши:

- Выделение/отмена выделения файлов. Использую клавишу «ins» и выделяю необходимые файлы, выделенные желтым цветом: (рис. -@fig:012 ).

![Выделение/отмена выделения файлов](image/12.png)

{ #fig:012 width=70% }

Для выделения файлов или его отмены можно использовать также команды «Отметить группу», «Снять отметку», «Обратить выделение» в меню «Файл»: (рис. -@fig:013 ).

![выделение/отмена выделения файлов](image/13.png)

{ #fig:013 width=70% }

- Копирование/перемещение файлов. Для копирования файла используется клавиша «F5»: (рис. -@fig:014 ).

![Копировние/перемещение файлов](image/14.png)

{ #fig:014 width=70% }

Для перемещения файла использовала клавишу «F6» (иллюстрация на рис. -@fig:015 )

![Перемещение файлов](image/15.png)

{ #fig:015 width=70% }

- Получение информации о размере и правах доступа на файлы и/или каталоги. Для получения данной информации можно перейти в команды: «Левая панель» → «Информация» (рис. -@fig:016 ).

![Информация о данном файле](image/16.png)

{ #fig:016 width=70% }

«Левая панель» → «Формат списка» → «Расширенный» ( рис. -@fig:017 , -@fig:018 , -@fig:019 ).

![Формат списка в mc](image/17.png)

{ #fig:017 width=70% }

![Формат списка файлов](image/18.png)

{ #fig:018 width=70% }

![Расширенный список](image/20.png)

{ #fig:019 width=70% }

«Файл» → «Права доступа» (рис. -@fig:020 , -@fig:021 ).

![Права доступа в mc](image/21.png)

{ #fig:020 width=70% }

![Команда chmod](image/22.png)

{ #fig:021 width=70% }

«Файл» → «Права (расширенные)» (рис. -@fig:022 , -@fig:023 ).

![Права (расширенные) в mc](image/23.png)

{ #fig:022 width=70% }

![Расширенная команда chown](image/24.png)

{ #fig:023 width=70% }

4. Далее выполнили основные команды меню правой панели (рис. -@fig:024 ).

![Правая панель в mc](image/25.png)

{ #fig:024 width=70% }

- Пункт «Список файлов» отображает размер файла и время его правки (рис. -@fig:025 ).

![Список файлов](image/26.png)

{ #fig:025 width=70% }

- Пункт «Быстрый просмотр» нужен для предпросмотра содержания файла (рис. -@fig:026, -@fig:027 ).

![Выбор опции](image/27.png)

{ #fig:026 width=70% }

![Быстрый просмотр](image/28.png)

{ #fig:027 width=70% }

- Пункт «Информация» отображает подробные данные о файле (рис. -@fig:028 , -@fig:029).

![Выбор опции](image/29.png)

{ #fig:028 width=70% }

![Информация о данном файле/каталоге](image/30.png)

{ #fig:029 width=70% }

- Пункт «Дерево» необходим для просмотра дерева каталога (отображает минимум информации) (рис. fig:030 ).

![Дерево каталога](image/30.png)

{ #fig:029 width=70% }

- Пункт «Формат списка» − «Укороченный» отображает только имя файла или каталога (видна минимальная информация) (Рис. -@fig:031 , -@fig:032 ).

![Формат списка (укороченный) в mc](image/31.png)

{ #fig:031 width=70% }

![Формат списка (укороченный)](image/32.png)

{ #fig:032 width=70% }

- Пункт «Формат списка» − «Расширенный» отображает подробную информацию о файлах, но менее подробную,чем пункт «Информация» (рис. -@fig:033,-@fig:034  ).

![Формат списка (расширенный) в mc](image/33.png)

{ #fig:033 width=70% }

![Формат списка (расширенный)](image/34.png)

{ #fig:034 width=70% }

- Пункт «Формат списка» − «Определенный пользователем» предоставляетпользователю возможность самому изменять степень подробности информации о файле, но она будет менее подробной, чем в пункте "Информация".

![Формат списка (определённый пользователем) в mc](image/33.png)

{ #fig:033 width=70% }

![Формат списка (определённый пользователем)](image/34.png)

{ #fig:034 width=70% }

- Пункт «Формат списка» − «Стандартный» ставится по умолчанию 

-  Пункт «Порядок сортировки» необходим для сортировки файлов или каталогов по конкретному критерию (рис. -@fig:035, -@fig:036, -@fig:037 ).

![Выбор опции](image/37.png)

{ #fig:035 width=70% }

![Настройки сортировки](image/38.png)

{ #fig:036 width=70% }

![Список отсортированных файлов](image/39.png)

{ #fig:037 width=70% }

- Пункт «Фильтр» необходим, чтобы просматривать название файлов или каталогов, которые подходят под указанную маску (рис. -@fig:038 ).

![Фильтр](image/40.png)

{ #fig:038 width=70% }

- Пункт "Выбор кодировки" нужен для просмотра и смены кодировки (рис. -@fig:039,-@fig:040 ).

![Выбор опции](image/41.png)

{ #fig:039 width=70% }

![Выбор кодировки](image/42.png)

{ #fig:040 width=70% }

5. Используя возможности под меню «Файл» (рис. -@fig:041), выполним:

![Выбор кодировки](image/43.png)

{ #fig:040 width=70% }

- Просмотр содержимого текстового файла/каталога. Выберем каталог bin и перейдем в пункт «Просмотр» (рис. -@fig:042).

![Просмотр каталога](image/44.png)

{ #fig:040 width=70% }

- Редактирование содержимого текстового файла april (без сохранения результатов
редактирования) . Перейдем в пункт «Правка» (рис. -@fig:043 ) и изменим содержание файла (рис. -@fig:044).

![Правка](image/45.png)

{ #fig:043 width=70% }

![Редактирование содержимого текстового файла april](image/46.png)

{ #fig:044 width=70% }

- Создание каталога. Далее перешли в пункт «Создание каталога» (рис. -@fig:045) и создали каталог "abc" (рис. -@fig:046, рис. -@fig:047)

![Выбор опции](image/47.png)

{ #fig:045 width=70% }

Создание каталога{ #fig:042 width=70% }

![Выбор названия файла](image/48.png)

{ #fig:046 width=70% }

![Содержимое каталога](image/49.png)

{ #fig:047 width=70% }

-  Копирование файлов в созданный каталог. Для этого выбрали файл april_0 (рис. -@fig:048,-@fig:049, -@fig:050 ).

![Выбор опции](image/50.png)

{ #fig:048 width=70% }

![Указываем путь в каталог для копирования](image/51.png)

{ #fig:049 width=70% }

![Проверка копирования](image/52.png)

{ #fig:050 width=70% }

6. Используя соответствующие средства под меню «Команда» (Скриншот -@fig:051 ), осуществим:

![Поиск в mc](image/53.png)

{ #fig:051 width=70% }

- Поиск в файловой системе файла с заданными условиями. Перешли в пункт «Поиск файла», задалаи следующие параметры: «От каталога» /,«Шаблон имени» *.с, «Содержимое» main (см. рис. -@fig:052 ) и осуществили поиск нужных файлов (см. рис. -@fig:053 ).

![Задание параметров поиска](image/54.png)

{ #fig:052 width=70% }

![Поиск файлов с расширением .c](image/55.png)

{ #fig:053 width=70% }


Аналогичным образом нашли файлы с шаблоном имени *.cpp (Рисунки -@fig:054 , -@fig:055 ).

![Задание параметров поиска](image/56.png)

{ #fig:054 width=70% }

![Поиск файлов с расширением .cpp](image/57.png)

{ #fig:055 width=70% }

- Выбор и повторение одной из предыдущих команд. Перешли в пункт «История командной строки» и увидила, что внизу экрана ничего не появилось (точнее - сноска «История»), т.к. командная строка не была использована  (Рисунок -@fig:056 ).

![Выбор опции](image/58.png)

{ #fig:056 width=70% }

- Переход в домашний каталог. Для перехода в домашний каталог перешли в пункт «Дерево каталогов» (рис. -@fig:057 ), выбрала необходимый каталог и нажала «enter», в результате чего, в левой панели перешла в домашний каталог (рис. -@fig:058 ).

![Выбор опции](image/60.png)

{ #fig:057 width=70% }

![Переход в домашний каталог](image/61.png)

{ #fig:058 width=70% }

- Анализ файла меню и файла расширений. Перешла в пункт «Редактировать файл расширений» (рис. -@fig:059,  -@fig:060 ). "Редактировать файл расширений" − позволяет задать с помощью определённого синтаксиса действия при запуске файлов с определённым расширением. Пункт «Редактировать файл меню» − позволяет отредактировать контекстное меню пользователя (рис. -@fig:061,  -@fig:062 ).

![Выбор опции](image/63.png)

{ #fig:059 width=70% }

![Редактирование файла расширений](image/64.png)

{ #fig:060 width=70% }

![Выбор опции](image/65.png)

{ #fig:061 width=70% }

![Редактирование файла расширений](image/66.png)

{ #fig:062 width=70% }

7. Далее вызвали под меню «Настройки» (Скриншот -@fig:063 ). Освоили операции, определяющие структуру экрана mc:

![Настройки](image/67.png)

{ #fig:063 width=70% }

- Перешли в пункт «Конфигурация» (Скриншот -@fig:064 ). Этот пункт позволяет скорректировать настройки работы с панелями.

![Параметры конфигурации](image/68.png)

{ #fig:064 width=70% }


- Перешли в пункт «Внешний вид» (иллюстрация на рис. -@fig:065 ), а затем в пункт «Настройки панелей» (иллюстрация на рис. -@fig:066 ). Данные пункты определяют элементы (строка меню,командная строка,подсказк и ипрочее), отображаемые при вызове mc,а также геометрию расположения панелей и цветовыделение.

![Настройка внешнего вида](image/70.png)

{ #fig:065 width=70% }

![Настройка панелей](image/72.png)

{ #fig:066 width=70% }

- Перешли в пункт «Подтверждение» (Рисунок -@fig:067 ).Этот пункт позволяет установить или убрать вывод окна с запросом подтверждения действий при операциях удаления и перезаписи файлов, атакже при выходе из программы.

![Настройка подтверждения](image/74.png)

{ #fig:067 width=70% }

- Перешли в пункт «Оформление» (Рисунок -@fig:068 ). Данный пункт позволяет поменять цветовую гамму визуальной оболочки для комфортной работы.

![Настройка оформления](image/76.png)

{ #fig:068 width=70% }

- Перешли в пункт «Биты символов» (Рисунок -@fig:069 ). Этот пункт задаёт формат обработки информации локальным терминалом.

![Настройка битов символов](image/78.png)

{ #fig:069 width=70% }

- Перешли в пункт «Распознавание клавиш» (Рисунок -@fig:070 ). Данное диалоговое окно используется для тестирования функциональных клавиш, клавишу правления курсором и прочее.

![Настройка распозанвания клавиш](image/80.png)

{ #fig:070 width=70% }

- Перешли в пункт «Виртуальные ФС» (Рисунок -@fig:071 ).Это настройки виртуальной файловой системы: тайм-аут,п ароль и прочее.
![Настройка виртуальных ФС](image/82.png)

{ #fig:071 width=70% }

- Перешла в пункт «Сохранить настройки» (Рисунок -@fig:072 ).Данный пункт сохранит все изменения.

![Сохранение настроек](image/83.png)

{ #fig:072 width=70% }


**Работа по встроенному редактору mc:**

1. С помощью команды «touch text.txt» создаем текстовой файл text.txt. Командой« ls» проверяем правильность выполненных действий  (рис. -@fig:073 ).

![Работа с консолью](image/84.png)

{ #fig:073 width=70% }

2. Открываем этот файл с помощью встроенного mc редактора командой «mcedit text.txt»(рис. -@fig:074 ).

![Работа с консолью](image/85.png)

{ #fig:074 width=70% }

3. Вставили в открытый файл небольшой фрагмент текста, скопированный из Интернета (Рисунок -@fig:075 ).

![Файл text.txt](image/86.png)

{ #fig:075 width=70% }

4.Выполним следующие действия:

- Удалим строку текста с помощью клавиши «F8» (Рисунки -@fig:076 , -@fig:077).

![Текст со строкой](image/87.png)

{ #fig:76 width=70% }

![Удаление строки](image/88.png)

{ #fig:077 width=70% }

- Выделили фрагмент текста, нажав «F3» для начала выделения текста и для его окончания, и скопировали его на новую строку, используя клавишу «F5» (Рисунки -@fig:078 , -@fig:079).

![Выделение фрагмента текста](image/89.png)

{ #fig:78 width=70% }

![Копирование фрагмента текста](image/90.png)

{ #fig:079 width=70% }

- Выделили фрагмент текста и перенесли его на новую строку с помощью клавиши «F6» (Рисунок -@fig:080).

![Выделение фрагмента текста](image/91.png)

{ #fig:080 width=70% }

- Сохранили файл, нажав «F2» (Рис. -@fig:081).

![Сохранение файла](image/92.png)

{ #fig:081 width=70% }

- Отменили последнее действие с помощью сочетания клавиш «ctrl»+«u» (Рисунок -@fig:082 ).

![Отмена действия](image/93.png)

{ #fig:082 width=70% }

- Перешли в конец файла, нажав клавиши «ctrl»+«end» (переход в конец файла), и написали следующий текст: «Лабораторная работа №7» (рис. -@fig:083 ).

![Переход в конец файла и написание текста ](image/94.png)

{ #fig:083 width=70% }

- Перешли в начало файла, нажав клавиши «ctrl»+«home» (переход в начало файла), и написалаи следующий текст: «Лабораторная работа №7» (рис. -@fig:084 ).

![Пишем текст в файл](image/95.png)

{ #fig:084 width=70% }

- Выполнила сохранение файла (клавиша «F2») и выйдем из него (клавиша «F10») (Рисунок -@fig:085).

![Сохранение файла](image/96.png)

{ #fig:085 width=70% }

5. Открыли файл с исходным текстом на языке программирования С. Открыли файл в редакторе mc с помощью команды «mc» (перед этим выстроила путь к файлу на консоли) (Рисунки -@fig:086 )

![Текст программы в mc](image/100.png)

{ #fig:086 width=70% }

6. Используя меню редактора «Команда» → «Включить/выключить подсветку синтаксиса», выключим подсветку синтаксиса (Рисунок -@fig:087, -@fig:088).

![Выключение подсветки](image/101.png)

{ #fig:087 width=70% }

![Выключение подсветки](image/102.png)

{ #fig:088 width=70% }

# Вывод

В процессе выполнения лабораторной работы №7 мы освоили основные возможности командной оболочки Midnight Commander и приобрели навыки практической работы по просмотру каталогов и файлов, а также манипуляций с ними.

# Ответы на контрольные вопросы

1. Панели могут дополнительно быть переведены в один из двух режимов: «Информация» или «Дерево». В режиме «Информация» на панель выводятся сведения о файле и текущей файловой системе, расположенных на активной панели. В режиме «Дерево» на одной из панелей выводится структура дерева каталогов.

2. Как с помощью команд shell, так и с помощью меню (комбинаций клавиш) mc можно выполнить следующие операции с файлами:

- копирование «F5» («cp имя_файла имя_каталога (в который копируем)») (Рисунок14)

- перемещение/переименование «F6» («mv имя_файла имя_каталога (в который перемещаем)»)(Рисунок15)

- создание каталога «F7» («mkdir имя_каталога»)(Рисунок38)

- удаление «F8» («rm имя_файла»)

- изменение прав доступа «ctrl+x» («chmod u+x имя_файла»)

3. Перейти в строку меню панелей mc можно с помощью функциональной клавиши «F9». В строке меню имеются пять меню: «Леваяпанель», «Файл», «Команда», «Настройки» и «Праваяпанель».
Под пункт меню «Быстрый просмотр» позволяет выполнить быстрый просмотр содержимого панели.

Подпункт меню «Информация» позволяет посмотреть информацию о файле или каталоге. В меню каждой (левой или правой) панели можно выбрать «Формат списка»:

- стандартный − выводит список файлов и каталогов с указанием размера и времени правки;

- ускоренный − позволяет задать число столбцов, на которые разбивается панель при выводе списка имён файлов или каталогов без дополнительной информации;

- расширенный − помимо названия файла или каталога выводит сведения о правах доступа, владельце, группе, размере, времени правки;

- определённый пользователем − позволяет вывести те сведения о файле или каталоге, которые задаст сам пользователь.

Подпункт меню «Порядок сортировки» позволяет задать критерии сортировки при выводе списка файлов и каталогов: без сортировки, по имени, расширенный, время правки, время доступа, время изменения атрибута, размер, узел.

4. Команды меню «Файл»:
- Просмотр(«F3»)− позволяет посмотреть содержимое текущего (или выделенного) файла без возможности редактирования.

- Просмотр вывода команды («М»+«!»)− функция запроса команды с параметрами (аргумент к текущему выбранному файлу).

- Правка(«F4») − открывает текущий (или выделенный) файл для его редактирования.

- Копирование(«F5»)− осуществляет копирование одного или нескольких файлов или каталогов в указанное пользователем во всплывающем окне место.

- Права доступа («Ctrl-x»«c»)− позволяет указать (изменить) права доступа к одному или нескольким файлам или каталогам.

- Жёсткая ссылка («Ctrl-x»«l»)− позволяет создать жёсткую ссылку к текущему(или выделенному) файлу.

- Символическая ссылка («Ctrl-x»«s»)− позволяет создать символическую ссылку к текущему (или выделенному) файлу.

- Владелец/группа («Ctrl-x»«o»)− позволяет задать (изменить) владельца и имя группы для одного или нескольких файлов или каталогов.

- Права(расширенные)− позволяет изменить права доступа и владения для одного или нескольких файлов или каталогов.

- Переименование («F6»)− позволяет переименовать (или переместить) один или несколько файлов или каталогов.

- Создание каталога («F7») − позволяет создать каталог.

- Удалить («F8») − позволяет удалить один или несколько файлов или каталогов.

- Выход («F10») − завершает работу mc.

5. Меню Команда
В меню Команда содержатся более общие команды для работы с mc.

Команды меню Команда:

- Дерево каталогов − отображает структуру каталогов системы.

- Поиск файла − выполняет поиск файлов по заданным параметрам.

- Переставить панели − меняет местами левую и правую панели.

- Сравнить каталоги («Ctrl-x»«d») − сравнивает содержимое двух каталогов.

- Размеры каталогов − отображает размер и время изменения каталога (по умолчанию в mc размер каталога корректно не отображается).

- История командной строки − выводит на экран список ранее выполненных в оболочке команд.

- Каталоги быстрого доступа(Ctrl-\»)− при вызове выполняется быстрая смена текущего каталога на один из заданного списка.

- Восстановление файлов − позволяет восстановить файлы на файловых системах ext2 и ext3.

- Редактировать файл расширений − позволяет задать с помощью определённого синтаксиса действия при запуске файлов с определённым расширением (например, какое программное обеспечение запускать для открытия или редактирования файлов с расширением doc или docx).

- Редактировать файл меню − позволяет отредактировать контекстное меню пользователя, вызываемое по клавише «F2».

- Редактировать файл расцветки имён − позволяет подобрать оптимальную для пользователя расцветку имён файлов в зависимости от их типа.

6. Меню Настройки содержит ряд дополнительных опций по внешнему виду и функциональности mc.
Меню Настройки содержит:

- Конфигурация − позволяет скорректировать настройки работы с панелями.

- Внешний вид и Настройки панелей − определяет элементы (строка меню, командная строка, подсказки и прочее), отображаемые при вызове mc, а также геометрию расположения панелей и цветовыделение.

- Биты символов − задаёт формат обработки информации локальным терминалом.

- Подтверждение − позволяет установить или убрать вывод окна с запросом подтверждения действий при операциях удаления и перезаписи файлов, а также при выходе из программы.

- Распознание клавиш − диалоговое окно используется для тестирования функциональных клавиш, клавиш управления курсором и прочее.

- Виртуальные ФС − настройки виртуальной файловой системы: тайм-аут, пароль и прочее.

7. Функциональные клавиши mc:
F1 – вызов контекстно-зависимой подсказки

F2 – вызов пользовательского меню с возможностью создания и/или дополнения дополнительных функций

F3 – просмотр содержимого файла, на который указывает подсветка в активной панели (без возможности редактирования)

F4 – вызов встроенного в mc редактора для изменения содержания файла, на который указывает подсветка в активной панели

F5 – копирование одного или нескольких файлов, отмеченных впервой (активной) панели, в каталог, отображаемый на второй панели

F6 – перенос одного или нескольких файлов, отмеченных в первой (активной) панели, в каталог, отображаемый на второй панели

F7 – создание подкаталога в каталоге, отображаемом в активной панели

F8 – удаление одного или нескольких файлов (каталогов), отмеченных в первой (активной) панели файлов

F9 – вызов меню mc

F10 – выход из mc

8. Встроенный в mc редактор вызывается с помощью функциональной клавиши «F4». В нём удобно использовать различные комбинации клавиш при редактировании содержимого (как правило текстового) файла. Клавиши для редактирования файла:
«Ctrl-y» − удалить строку

«Ctrl-u» − отмена последней операции

«ins» - вставка/замена

«F7» − поиск (можно использовать регулярные выражения)

«↑-F7» − повтор последней операции поиска

«F4» − замена

«F3» − первое нажатие − начало выделения, второе − окончание выделения

«F5» − копировать выделенный фрагмент

«F6» − переместить выделенный фрагмент

«F8» − удалить выделенный фрагмент

«F2» − записать изменения в файл

«F10» − выйти из редактор

9. Для редактирования меню пользователя, которое вызывается клавишей «F2», необходимо перейти в пункт «Редактировать файл меню» → «Команда» и изменить настройки файла.

10. Часть команд «Меню пользователя», а также меню «Файл» позволяют выполнять действия, определяемые пользователем, над текущим файлом. Например, копирование каталога или файла, переименование, перемещение, архивирование.
11. 