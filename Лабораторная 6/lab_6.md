---
## Front matter
title: "Отчет по лабораторной работе №6"
subtitle: "Решение моделей в непрерывном и дискретном времени"
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

Основной целью работы является освоение специализированных пакетов для решения задач в непрерывном и дискретном времени.

# Задание

1. Используя Jupyter Lab, повторите примеры из раздела 6.2.
2. Выполните задания для самостоятельной работы (раздел 6.4).

# Выполнение лабораторной работы

**1.** Для начала я повторила все примеры. Тут их не так много. Первый пример это модель экспоненциального роста. Для решения обыкновенных дифференциальных уравнений (ОДУ) в Julia можно использовать пакет diffrentialEquations.jl. Численное решение в Julia будет иметь следующий вид:
(рис. [-@fig:001]) 

![Модель экспоненциального роста. Численное решение.](image/1.png){ #fig:001 width=70% }

Далее получила графика, соответствующий полученному решению:
(рис. [-@fig:002]) 

![Модель экспоненциального роста. График.](image/2.png){ #fig:002 width=70% }

Если требуется задать точность решения, то можно воспользоваться параметрами
abstol (задаёт близость к нулю) и reltol (задаёт относительную точность). (рис. [-@fig:003]) 

![Модель экспоненциального роста. График с точным решением.](image/3.png){ #fig:003 width=70% }

**2.** Далее рассмотрела систему Лоренца. Численное решение в Julia будет иметь следующий вид:
(рис. [-@fig:004]) (рис. [-@fig:005]) (рис. [-@fig:006])  

![Аттрактор Лоренца. Численное решение t.](image/4.png){ #fig:004 width=70% }
![Аттрактор Лоренца. Численное решение u(t).](image/5.png){ #fig:005 width=70% }
![Аттрактор Лоренца. График.](image/6.png){ #fig:006 width=70% }

Можно отключить интерполяцию. (рис. [-@fig:007]) 

![Аттрактор Лоренца. График с отключенной интерполяцией.](image/7.png){ #fig:007 width=70% }

**3.** Рассмотрела Модель Лотки–Вольтерры. Модель Лотки–Вольтерры описывает взаимодействие двух видов типа «хищник – жертва», где x - количество жертв, y — количество хищников, t — время, alfa, beta, gamma, delta — коэффициенты, отражающие взаимодействия между видами (в данном случае alfa — коэффициент рождаемости жертв, gamma — коэффициент убыли хищников, beta — коэффициент убыли жертв в результате взаимодействия с хищниками, delta — коэффициент роста численности хищников). Численное решение в Julia будет иметь следующий вид:
(рис. [-@fig:008]) (рис. [-@fig:009]) 

![Модель Лотки–Вольтерры: динамика изменения численности популяций](image/8.png){ #fig:008 width=70% }

![ Модель Лотки–Вольтерры: фазовый портрет](image/9.png){ #fig:009 width=70% }

**10.** Приступила к заданиям для самостоятельной работы. Нумерация соответствует.

- Задание 1 (рис. [-@fig:010]) (рис. [-@fig:011]) (рис. [-@fig:012]) (рис. [-@fig:013]) 

![Задание 1. Код](image/10.png){ #fig:010 width=70% }

![Задание 1. График](image/11.png){ #fig:011 width=70% }

![Задание 1. Код анимации](image/12.png){ #fig:012 width=70% }

![Задание 1. Анимация](image/13.gif){ #fig:013 width=70% }

- Задание 2 (рис. [-@fig:014]) (рис. [-@fig:015]) (рис. [-@fig:016]) (рис. [-@fig:017]) 

![Задание 2. Код](image/14.png){ #fig:014 width=70% }

![Задание 2. График](image/15.png){ #fig:015 width=70% }

![Задание 2. Код анимации](image/16.png){ #fig:016 width=70% }

![Задание 2. Анимация](image/17.gif){ #fig:017 width=70% }

- Задание 3 (рис. [-@fig:018]) (рис. [-@fig:019]) (рис. [-@fig:020]) (рис. [-@fig:021]) 

![Задание 3. Код](image/18.png){ #fig:018 width=70% }

![Задание 3. График](image/19.png){ #fig:019 width=70% }

![Задание 3. Код анимации](image/20.png){ #fig:020 width=70% }

![Задание 3. Анимация](image/21.gif){ #fig:021 width=70% }

- Задание 4 (рис. [-@fig:022]) (рис. [-@fig:023]) (рис. [-@fig:024]) (рис. [-@fig:025]) 

![Задание 4. Код](image/22.png){ #fig:022 width=70% }

![Задание 4. График](image/23.png){ #fig:023 width=70% }

![Задание 4. Код анимации](image/24.png){ #fig:024 width=70% }

![Задание 4. Анимация](image/25.gif){ #fig:025 width=70% }

- Задание 5 (рис. [-@fig:026]) (рис. [-@fig:027]) (рис. [-@fig:028])

![Задание 5. Код](image/26.png){ #fig:026 width=70% }

![Задание 5. График](image/27.png){ #fig:027 width=70% }

![Задание 5. Фазовый портрет](image/28.png){ #fig:028 width=70% }

- Задание 6 (рис. [-@fig:029]) (рис. [-@fig:030]) (рис. [-@fig:031]) (рис. [-@fig:032]) 

![Задание 6. Код](image/29.png){ #fig:029 width=70% }

![Задание 6. График](image/30.png){ #fig:030 width=70% }

![Задание 6. Код анимации](image/31.png){ #fig:031 width=70% }

![Задание 6. Анимация](image/32.gif){ #fig:032 width=70% }

- Задание 7 (рис. [-@fig:033]) (рис. [-@fig:034]) (рис. [-@fig:035]) (рис. [-@fig:036]) (рис. [-@fig:037]) (рис. [-@fig:038]) (рис. [-@fig:039])

![Задание 7. Код](image/33.png){ #fig:033 width=70% }

![Задание 7. График](image/34.png){ #fig:034 width=70% }

![Задание 7. Фазовый портрет](image/35.png){ #fig:035 width=70% }

![Задание 7. Код анимация для графика](image/36.png){ #fig:036 width=70% }

![Задание 7. Анимация графика](image/37.gif){ #fig:037 width=70% }

![Задание 7. Код анимация для фазового портрета](image/38.png){ #fig:038 width=70% }

![Задание 7. Анимация фазового портрета](image/39.gif){ #fig:039 width=70% }

- Задание 8 (рис. [-@fig:040]) (рис. [-@fig:041]) (рис. [-@fig:042]) (рис. [-@fig:043]) (рис. [-@fig:044]) (рис. [-@fig:045]) (рис. [-@fig:046])

![Задание 8. Код](image/40.png){ #fig:040 width=70% }

![Задание 8. График](image/41.png){ #fig:0341 width=70% }

![Задание 8. Фазовый портрет](image/42.png){ #fig:042 width=70% }

![Задание 8. Код анимация для графика](image/43.png){ #fig:043 width=70% }

![Задание 8. Анимация графика](image/44.gif){ #fig:044 width=70% }

![Задание 8. Код анимация для фазового портрета](image/45.png){ #fig:045 width=70% }

![Задание 8. Анимация фазового портрета](image/46.gif){ #fig:046 width=70% }

# Вывод

Освоила специализированные пакеты для решения задач в непрерывном и дискретном времени.