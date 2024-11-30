---
## Front matter
title: "Отчет по лабораторной работе №3"
subtitle: "Управляющие структуры"
author: "Легиньких Галина Андреевна"

## Generic otions
lang: ru-RU
toc-title: "Содержание"
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

Основная цель работы — освоить применение циклов функций и сторонних для Julia пакетов для решения задач линейной алгебры и работы с матрицами.

# Задание

1. Используя Jupyter Lab, повторите примеры из раздела 2.2.
2. Выполните задания для самостоятельной работы (раздел 2.4).

# Выполнение лабораторной работы

**1.** Для начала я изучила видеоматериал к лекции и повторила примеры из раздела 3.2. Сначало это были циклы while и for. Для различных операций, связанных с перебором индексируемых элементов структур данных, традиционно используются циклы while и for. (рис. [-@fig:001]) (рис. [-@fig:002]) (рис. [-@fig:003])

![while](image/1.png){ #fig:001 width=70% }

![for вналогично while](image/2.png){ #fig:002 width=70% }

![for массивы](image/3.png){ #fig:003 width=70% }

**2.** Условные выражения. Довольно часто при решении задач требуется проверить выполнение тех или иных условий. Для этого используют условные выражения. Повторила синтаксис условных выражений с тернарными операторами. (рис. [-@fig:004])

![Условные выражения](image/4.png){ #fig:004 width=70% }

**3.** Далее перешла к функциям. Julia дает нам несколько разных способов написать функцию. Первый требует ключевых
слов function и end. (рис. [-@fig:005])

![Функции 1-ый способ](image/5.png){ #fig:005 width=70% }

В качестве альтернативы, можно объявить любую из выше определённых функций
в одной строке. (рис. [-@fig:006])

![Функции 2-ой способ](image/6.png){ #fig:006 width=70% }

Наконец, можно объявить выше определённые функции как "анонимные". (рис. [-@fig:007])

![Функции 3-ий способ](image/7.png){ #fig:007 width=70% }

По соглашению в Julia функции, сопровождаемые восклицательным знаком, изменяют свое содержимое, а функции без восклицательного знака не делают этого. (рис. [-@fig:008])

![sort as !sort](image/8.png){ #fig:008 width=70% }

В Julia функция map является функцией высшего порядка, которая принимает функцию в качестве одного из своих входных аргументов и применяет эту функцию к каждому элементу структуры данных, которая ей передаётся также в качестве аргумента. (рис. [-@fig:009])

![map](image/9.png){ #fig:009 width=70% }

Функция broadcast — ещё одна функция высшего порядка в Julia, представляющая собой обобщение функции map.Функция broadcast() будет пытаться привести все объекты к общему измерению, map() будет напрямую применять данную функцию поэлементно. (рис. [-@fig:010])

![broadcast](image/10.png){ #fig:010 width=70% }

**4.** Julia имеет более 2000 зарегистрированных пакетов, что делает их огромной частью экосистемы Julia. Научилась загружать пакеты. (рис. [-@fig:011])

![Загрузка пакетов](image/11.png){ #fig:011 width=70% }

И использовать их. (рис. [-@fig:012])

![Использование пакетов](image/12.png){ #fig:012 width=70% }

**5.** Перешла к заданиям для самостоятельной работы. Дублировать задания не буду, они слишком большие. Нумерация соответствует нумерации в файле задания. 

- Задание 1.1 с помощью while (рис. [-@fig:013])

![Задание 1.1 while](image/13.png){ #fig:013 width=70% }

- Задание 1.1 с помощью for (рис. [-@fig:014])

![Задание 1.1 for](image/14.png){ #fig:014 width=70% }

- Задание 1.2 (рис. [-@fig:015])

![Задание 1.2](image/15.png){ #fig:015 width=70% }

- Задание 1.3 (рис. [-@fig:016])

![Задание 1.3](image/16.png){ #fig:016 width=70% }

- Задание 2 (рис. [-@fig:017])

![Задание 2](image/17.png){ #fig:017 width=70% }

- Задание 3 (рис. [-@fig:018])

![Задание 3](image/18.png){ #fig:018 width=70% }

- Задание 4 (рис. [-@fig:019])

![Задание 4](image/19.png){ #fig:019 width=70% }

- Задание 5 (рис. [-@fig:020])

![Задание 5](image/20.png){ #fig:020 width=70% }

- Задание 6 (рис. [-@fig:021])

![Задание 6](image/21.png){ #fig:021 width=70% }

- Задание 7.0 (рис. [-@fig:022])

![Задание 7.0](image/22.png){ #fig:022 width=70% }

- Задание 7.1 (рис. [-@fig:023])

![Задание 7.1](image/23.png){ #fig:023 width=70% }

- Задание 7.2 (рис. [-@fig:024])

![Задание 7.2](image/24.png){ #fig:024 width=70% }

- Задание 7.3 (рис. [-@fig:025])

![Задание 7.3](image/25.png){ #fig:025 width=70% }

- Задание 7.4 (рис. [-@fig:026])

![Задание 7.4](image/26.png){ #fig:026 width=70% }

- Задание 8.1 - 8.2 (рис. [-@fig:027])

![Задание 8.1 - 8.2](image/27.png){ #fig:027 width=70% }

- Задание 8.3 - 8.4 (рис. [-@fig:028])

![Задание 8.3 - 8.4](image/28.png){ #fig:028 width=70% }

- Задание 8.5 (рис. [-@fig:029])

![Задание 8.5](image/29.png){ #fig:029 width=70% }

- Задание 9 (рис. [-@fig:030])

![Задание 9](image/30.png){ #fig:030 width=70% }

- Задание 10.1 - 10.2 (рис. [-@fig:031])

![Задание 10.1 - 10.2](image/31.png){ #fig:031 width=70% }

- Задание 10.3 (рис. [-@fig:032])

![Задание 10.3](image/32.png){ #fig:032 width=70% }

- Задание 11 (рис. [-@fig:033])

![Задание 11](image/33.png){ #fig:033 width=70% }

# Вывод

Освоила применение циклов функций и сторонних для Julia пакетов для решения задач линейной алгебры и работы с матрицами.