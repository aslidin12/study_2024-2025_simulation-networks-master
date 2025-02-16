---
## Front matter
title: "Моделирование сетей передачи данных"
subtitle: "Отчёт по лабораторной работе №1: Введение в Mininet"
author: "Ахлиддинзода Аслиддин"

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
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---
# Цель работы

Основной целью работы является развёртывание в системе виртуализации
(например, в VirtualBox) mininet, знакомство с основными командами для работы с Mininet через командную строку и через графический интерфейс.

# Выполнение лабораторной работы

1. Добавим для mininet указание на использование двух адаптеров при запуске.

![Добавление для mininet указание на использование двух адаптеров при запуске.](image/1.PNG)

2. Проверим номер установленной версии mininet.

![Проверим номер установленной версии mininet.](image/2.PNG)

3. Здесь выбираем системный моноширинный шрифт, кегль шрифта — 12 пунктов.

![Выбираем системный шрифт.](image/3.PNG)

4. Проверим подключение между хостами h1 и h2 с помощью команды ping.

![Проверка подключения между хостами.](image/4.PNG)


# Вывод

В ходе выполнения лабораторной работы получили навыки развертывания в системе виртуализации
(например, в VirtualBox) mininet, познакомились с основными командами для работы с Mininet через командную строку и через графический интерфейс.

# Список литературы. Библиография

[1] Mininet: https://mininet.org/