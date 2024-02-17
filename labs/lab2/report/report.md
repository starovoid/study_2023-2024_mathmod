---
## Front matter
title: "Отчёт по лабораторной работе №2"
subtitle: "Задача о погоне"
author: "Старовойтов Егор Сергеевич"

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
Решить путем математического моделирования задачу о погоне.

# Задание
1. Провести аналогичные образцовым рассуждения и вывод дифференциальных уравнений,
если скорость катера больше скорости лодки в n раз (значение n задайте
самостоятельно). В моем варианте под номером №51 `n = 5.1`.
2. Построить траекторию движения катера и лодки для двух случаев. (Задайте
самостоятельно начальные значения).



# Выполнение лабораторной работы
Я вывел уравнение: `dr/dtheta = r/sqrt(25.01)`, откуда `dr = r/sqrt(25.01)`.

На скриншотах ниже продемонстрирован набор команд в консоли Scilab для первого и второго случая задачи.

## Первый случай
![Скрипт](image/15-17-50.png){#fig:001 width=70%}

![График](image/15-17-58.png){#fig:002 width=70%}

Примерная точка пересечения катера с лодкой - (6, -6).

## Второй случай
![Скрипт](image/15-21-08.png){#fig:003 width=70%}

![График](image/15-21-04.png){#fig:004 width=70%}

Примерная точка пересечения катера с лодкой - (18, -16).



# Выводы
Путем математического моделирования в Scilab решена задача о погоне.
