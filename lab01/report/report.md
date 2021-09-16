---
# Front matter
lang: ru-RU
title: "Отчет по лабораторной работе №1"
subtitle: "Информационная безопасноть"
author: "Коломиец Мария Владимировна НПИбд-01-18"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
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
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the υalue makes tex try to haυe fewer lines in the paragraph.
  - \interlinepenalty=0 # υalue of the penalty (node) added after each line of a paragraph.
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
  - \usepackage{amsmath}
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Приобрести практические навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.


# Задание

Лабораторная работа подразумевает установку на виртуальную машину VirtualBox операционной системы Linux, дистрибутив Centos.

# Выполнение лабораторной работы

1. Создала новую виртуальную машину. Для этого в VirtualBox выбрала Машина Создать.
Указала имя виртуальной машины — Base, тип операционной системы — Linux, RedHat (рис. -@fig:001). Указала размер основной памяти виртуальной машины — 1024 МБ(рис. -@fig:002)

![Окно "Имя машины и тип ОС"](image/01.png){ #fig:001 width=70% height=70% }

![Окно "Размер основной памяти"](image/02.png){ #fig:002 width=70% height=70% }

2. Задала конфигурацию жёсткого диска — загрузочный, VDI (BirtualBox Disk Image), динамический виртуальный диск. (рис. -@fig:003), (рис. -@fig:004), (рис. -@fig:005). 

![Окно "Виртуальный жесткий диск"](image/03.png){ #fig:003 width=70% height=70% }

![Окно "Мастер создания нового виртульного диска"](image/04.png){ #fig:004 width=70% height=70% }

![Окно "Дополнительные атрибуты виртуального диска"](image/05.png){ #fig:005 width=70% height=70% }

3. Задала размер диска — 40 ГБ, его расположение. (рис. -@fig:006). 

![Окно "Расположение и размер виртуального диска"](image/06.png){ #fig:006 width=70% height=70% }

4. Проверила, какой путь имет папка для снимков виртуальной машины Base. (рис. -@fig:007) Выбрала в VirtualBox Свойства Носители виртуальной машины Base.
Добавила новый привод оптических дисков и выбрала образ. (рис. -@fig:008). 

![Окно «Свойства» виртуальной машины Base](image/07.png){ #fig:007 width=70% height=70% }

![Окно "Носители" виртуальной машины](image/08.png){ #fig:008 width=70% height=70% }

5. Запустила виртуальную машину Base, выбрала установку системы на жёсткий диск. (рис. -@fig:009). 

![Запуск установки системы](image/09.png){ #fig:009 width=70% height=70% }

6. Установила русский язык для интерфейса и раскладки клавиатуры (рис. -@fig:0010). 

![Установка русского языка](image/010.png){ #fig:0010 width=70% height=70% }

7. В качестве имени машины указала "mvkolomiets.localdomain" (рис. -@fig:0011). Указала часовой пояс «Москва» (рис. -@fig:0012). Произвела первичную настройку.  (рис. -@fig:0013).

![Задать сетевое имя виртуальной машины](image/011.png){ #fig:0011 width=70% height=70% }

![Указать часовой пояс «Москва»](image/012.png){ #fig:0012 width=70% height=70% }

![Обзор установки](image/013.png){ #fig:0013 width=70% height=70% }

8. Установила пароль для root (рис. -@fig:0014).

![Установка пароля для root](image/014.png){ #fig:0014 width=70% height=70% }

9. Создала пользователя mvkolomiets. (рис. -@fig:0015).

![Создание пользователя](image/015.png){ #fig:0015 width=70% height=70% }

10. Завершила установку операционной системы  и перезагрузила её. (рис. -@fig:0016).

![Виртуальная машина Base. Завершение установки](image/016.png){ #fig:0016 width=70% height=70% }

11. Запустила виртуальную машину Base и настроила её. (рис. -@fig:0017), (рис. -@fig:0018), (рис. -@fig:0019). 

![Информация о лицензии 1](image/017.png){ #fig:0017 width=70% height=70% }

![Информация о лицензии 2](image/018.png){ #fig:0018 width=70% height=70% }

![Виртуальная машина](image/019.png){ #fig:0019 width=70% height=70% }

12. Подключилась к виртуальной машине с помощью созданной учётной записи. На виртуальной машине Base запустила терминал, перешла под учетную запись root с помощью команды su. С помощью команды yum update обновила системные файлы и установила необходимые программы, например, mc: yum update, yum install mc. (рис. -@fig:0020), (рис. -@fig:0021). 

![Установка необходимых программ 1](image/020.png){ #fig:0020 width=70% height=70% }

![Установка необходимых программ 2](image/021.png){ #fig:0021 width=70% height=70% }

13. Для оптимизации работы в операционной системе установила необходимые драйвера. (рис. -@fig:0022), (рис. -@fig:0023), (рис. -@fig:0024), (рис. -@fig:0025). 

![Ввод пароля для суперюзера](image/022.png){ #fig:0022 width=70% height=70% }

![Установка необходимых драйверов](image/023.png){ #fig:0023 width=70% height=70% }

![Подключенный диск с драйверами](image/024.png){ #fig:0024 width=70% height=70% }

![Рабочая система](image/025.png){ #fig:0025 width=70% height=70% }


# Выводы
На основе проделанной работы приобрела практические навыки установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.