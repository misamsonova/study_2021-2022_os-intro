
---
## Front matter
lang: ru-RU
title: Краткий отчёт по лабораторной работе №4
author: Samsonova Maria, Student of RUDN University, Moscow, Russian Federation
institute: RUDN University, Moscow, Russian Federation

Date: 28-04-2022

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Цель выполнения лабораторной работы №4

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Ход выполнения лабораторной работы №4

1. Определяем полное имя нашего домашнего каталога с помощью команды pwd.
2. Переходим в каталог /tmp и выводим на экран содержимое каталога /tmp. Для этого используем  команду ls с различными опциями.
- Для того, чтобы отобразить имена скрытых файлов, необходимо использовать команду ls
с опцией a.
- Можно также получить информацию о типах файлов (каталог, исполняемый файл,
ссылка), для чего используем опцию F.
-  Получим подробный список, в котором будет отображаться владелец, группа, дата создания, размер и другие параметры с помощью команды ls и опции -l.
- Получим все файлы в каталогах, включая скрытые файлы, начинающиеся с точки, а также информацию о типе файла, права доступа к файлу, количество ссылок на файл, имя владельца, имя группы, размер файла в байтах и временной штамп (время последней модификации файла, если не задано другое).
3. Далее определяем, есть ли в каталоге /var/spool подкаталог с именем cron с помощью перехода в каталог /var/spool и просмотра содержимого каталога командой ls. Обнаруживаем, что папки cron нет.
4. Переходим в наш домашний каталог и выводим на экран его содержимое. Определяем, что владельцем файлов и подкаталогов является misamsonova.
5. В домашнем каталоге создаём новый каталог с именем newdir, переходим в каталог newdir и в каталоге ~/newdir создаём новый каталог с именем morefun.
- В домашнем каталоге создаём одной командой три новых каталога с именами
letters, memos, misk. Затем удаляем эти каталоги одной командой.
- Попробуем удалить ранее созданный каталог ~/newdir командой rm. Проверим, был ли каталог удалён. А также удаляем каталог ~/newdir/morefun из домашнего каталога. Проверим, был ли
каталог удалён.
6. С помощью команды man определим, какую опцию команды ls нужно использовать для просмотра содержимое не только указанного каталога, но и подкаталогов, входящих в него
7. Используем команду man для просмотра описания следующих команд: cd, pwd, mkdir,
rmdir, rm.
8. Получаем информацию о последовательности истории команд с помощью команды history и выполняем модификацию и исполнение нескольких команд из буфера команд с помощью команды ![номер выполнения команды из истории команд] (например, !99, !103, !95, !114 ).

# Итог выполнения лабораторной работы №4

В процессе выполнения лабораторной работы №4 мы приобрели практические навыки взаимодействия пользователя с системой посредством командной строки.

## {.standout}

***Спасибо за внимание!***
