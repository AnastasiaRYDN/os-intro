---
# Front matter
lang: ru-RU
title: "Лабораторная работа №5"
subtitle: "Основы интерфейса взаимодействия пользователя с системой Unix на уровне командной строки"
author: "Данилова Анастасия Сергеевна"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобретение практических навыков взаимодействия пользователя с системой посредством командной строки.

# Задание

1. Для начала ознакомимся с основными командами ОС типа Linux: man, cd, pwd, ls, history, mkdir, rm, прочитав данную нам информацию.
2. Далее воспользуемся командой ls c различными опциями и cd.
3. Создаем и удаляем каталоги согласно заданию.
4. С помощью команды man просматриваем опции предыдущих команд.


# Выполнение лабораторной работы

1. Для начала определим полное имя нашего каталога, использую команду pwd.

<img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис1.jpg" style="zoom:67%;" />

2.1 Переходим в каталог /tmp, используя команду cd и просматриваем содержимое каталога с помощью команды ls

<img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис2.jpg" style="zoom:67%;" />

2. 2 Также используем опцию а, которая отображает имена скрытых файлов

<img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис3.jpg" style="zoom:67%;" />

2.3 Определяем, что в каталоге /var/spool есть подкаталог с именем cron

<img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис4.jpg" style="zoom:67%;" />

2.4 Переходим в домашний каталог, выводим содержимое и видим имя владельца файлов и подкаталогов

<img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис5.jpg" style="zoom:67%;" />

3.1-3.2 В домашнем каталоге создаем новый каталог с именем newdir. В каталоге ~/newdir создаем новый каталог с именем morefun

<img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис6.jpg" style="zoom:67%;" />

3.3 Создаем три новых каталога *одной* командой mkdir и удаляем их также одной командой rm

<img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис7.jpg" style="zoom:67%;" />

3.4 -3.5 Для удаления каталога newdir необходимо использовать опцию r, далее проверяем, что каталог удалился

<img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис8.jpg" style="zoom:67%;" />

4. Опцию -l команды ls нужно использовать для просмотра всей информации содержимого не только указанного каталога, но и подкаталогов, входящих в него.

5.  Опции, позволяющие отсортировать по времени последнего изменения выводимый список содержимого каталога с развёрнутым описанием файлов: ls -lt, ls -ltr

6. Используем команду man для просмотра описания следующих команд: cd, pwd, mkdir, rmdir, rm. Основные опции cd:  -p разыменовывает символические ссылки, -l переходит по символическим ссылкам. Основные опции pwd: -L - брать директорию из переменной окружения; -P - отбрасывать все символические ссылки; --help - отобразить справку по утилите; --version - отобразить версию утилиты. Основные опции mkdir:  -m устанавливает права доступа для создаваемой директории;  -v выводить сообщение о каждой создаваемой директории. Основные опции rm: -i выводить запрос на подтверждение удаления каждого файла.

   <img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис9.jpg" style="zoom:67%;" />

   





   

7. При помощи команды history выполним модификацию. В данном случае изменим строку 65
8. <img src="C:\Users\nastd\Pictures\Camera Roll\лаб 5\рис10.jpg" style="zoom:67%;" />



**Выводы**

Я приобрела практические навыки взаимодействия пользователя с системой посредством командной строки. Также познакомилась с новыми командами.