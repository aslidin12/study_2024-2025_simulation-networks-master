---
## Front matter
title: "Моделирование сетей передачи данных"
subtitle: "Отчёт по лабораторной работе №2: Измерение и тестирование пропускной способности сети.Интерактивный эксперимент"
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

Основной целью работы является знакомство с инструментом для измерения
пропускной способности сети в режиме реального времени — iPerf3, а также
получение навыков проведения интерактивного эксперимента по измерению
пропускной способности моделируемой сети в среде Mininet.

# Выполнение лабораторной работы

1. Установили iperf3_plotter:

![Исправление прав запуска X-соединения в виртуальной машине mininet](image/1.PNG)

2. Зададим простейшую топологию, состоящую из двух хостов и коммутатора с назначенной по умолчанию mininet сетью 10.0.0.0/8

![Создание простейшей топологии](image/2.PNG)

3. Проведите простейший интерактивный эксперимент по измерению пропускной способности с помощью iPerf3:

![Отображение информации их сетевых интерфейсов и IP-адресов](image/3.PNG)


4. Для указания iPerf3 периода времени для передачи можно использовать ключ -t:

![Добавление 10% потерь пакетов к интерфейсу h1-eth0](image/5.PNG)

5. Настройте клиент iPerf3 для выполнения теста пропускной способности с 2-секундным интервалом времени

![Проверка](image/6.PNG)

6. Задаем на клиенте iPerf3 отправку определённого объёма данных.

![Добавление 10% потерь пакетов на хосте h2](image/7.PNG)

7. В тесте измерения пропускной способности iPerf3 изменили номер порта для отправки

![Проверка](image/8.PNG)

9. Восстановим конфигурацию по умолчанию, удалив все правила, применённые к сетевому планировщику соответствующего интерфейса

![Восстановление конфигурацию по умолчанию](image/9.PNG)

10. Останавливаем сервер

![Проверка](image/10.PNG)

11. Экспортировали результаты теста измерения пропускной способности iPerf3
в файл JSON:


![Добавление на узле h1 коэффициента потери пакетов 50%](image/12.PNG)


# Вывод

В ходе выполнения лабораторной работы познакомились с инструментом для измерения
пропускной способности сети в режиме реального времени — iPerf3, а также
получили навыки проведения интерактивного эксперимента по измерению
пропускной способности моделируемой сети в среде Mininet.


# Список литературы. Библиография

[1] Mininet: https://mininet.org/