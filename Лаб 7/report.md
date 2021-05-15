---
# Front matter
lang: ru-RU
title: "Лабораторная работа 7"
subtitle: "Поиск файлов. Перенаправление
ввода-вывода. Просмотр запущенных процессов"
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

Ознакомление с инструментами поиска файлов и фильтрации текстовых данных. Приобретение практических навыков: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем.

# Задание

1. Использование перенаправления ввода-вывода
2. Практика использования команды find для поиска файлов по каким-либо критериям
3. Фильтрация текста
4. Проверка использования диска
5. Управление задачами и процессами
6.  Получение информации о процессах


# Выполнение лабораторной работы

1. Осуществляем вход в систему
2. Записываем в файл file.txt названия файлов, содержащихся в каталоге /etc и дописываем в этот же файл названия файлов, содержащихся в вашем домашнем каталоге.
   ![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис1.jpg)
3. Выведем имена всех файлов из file.txt, имеющих расширение .conf       
   ![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис2.jpg)

![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис3.jpg)

4. С помощью команды ls -a | grep c* выясняем, что файл, который начинается с буквы c всего один. Также это можно сделать с помощью команды find ~ -name "f*" -print.
   ![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис4.jpg)

5. . Выводим на экран имена файлов из каталога /etc, начинающиеся с символа h. Для этого сначала перейдем в каталог  /etc и воспользуемся командой find
   ![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис5.jpg)

6. Запустиv в фоновом режиме процесс, который будет записывать в файл ~/logfile файлы, имена которых начинаются с log.
   ![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис6.jpg)

7. И удалим файл ~/logfile.(фото выше)

8. Запускаем из консоли в фоновом режиме редактор gedit (команда gedit &)
   ![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис7.jpg)

9. Определяем идентификатор процесса gedit, используя команду ps, конвейер и фильтр grep. Этот идентификатор более простым способом можно определить более простым способом с помощью команды jobs. 
   ![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис8.jpg)



10. Прочитав справку команды kill, используем её для завершения процесса gedit
    ![](C:\Users\nastd\Pictures\Camera Roll\лаб7\рис9.jpg)

11. Выполним команды df и du, предварительно получив более подробную информацию об этих командах, с помощью команды man. рис 10-11
    <img src="C:\Users\nastd\Pictures\Camera Roll\лаб7\рис10.jpg" style="zoom:67%;" />



<img src="C:\Users\nastd\Pictures\Camera Roll\лаб7\рис11.jpg" alt="РИС11" style="zoom:67%;" />



12. Воспользовавшись справкой команды find, выведем имена всех директорий, имеющихся в моем домашнем каталоге.
    <img src="C:\Users\nastd\Pictures\Camera Roll\лаб7\рис12.jpg" style="zoom:67%;" />



# Выводы

Я ознакомилась с инструментами поиска файлов и фильтрации текстовых данных. Приобрела практические навыки: по управлению процессами (и заданиями), по проверке использования диска и обслуживанию файловых систем. Познакомилась с новыми командами и их опциями.

