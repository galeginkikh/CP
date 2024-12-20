---
## Front matter
lang: ru-RU
title: Лабораторная работа №4
subtitle: "Линейная алгебра"
author:
  - Легиньких Г.А.
institute:
  - Российский университет дружбы народов, Москва, Россия

## i18n babel
babel-lang: russian
babel-otherlangs: english

## Formatting pdf
toc: false
toc-title: Содержание
slide_level: 2
aspectratio: 169
section-titles: true
theme: metropolis
header-includes:
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
---

# Информация

## Докладчик

:::::::::::::: {.columns align=center}
::: {.column width="70%"}

  * Легиньких Галина Андреевна
  * НФИбд-02-21
  * Российский университет дружбы народов
  * [1032216447@pfur.ru](mailto:1032216447@pfur.ru)
  * <https://github.com/galeginkikh>

:::
::: {.column width="30%"}

:::
::::::::::::::

# Основная информация

## Цель работы

Основной целью работы является изучение возможностей специализированных пакетов Julia для выполнения и оценки эффективности операций над объектами линейной алгебры.

## Задание

1. Используя Jupyter Lab, повторите примеры из раздела 4.2.
2. Выполните задания для самостоятельной работы (раздел 4.4).

# Выполнение

## Поэлементные операции над многомерными массивами

Примеры поэлементной суммы. 

Так же повторила примеры поэлементного произведения.

Для работы со средними значениями можно воспользоваться возможностями пакета Statistics.

![Поэлементная сумма](image/1.png){ #fig:001 width=50% }

## Транспонирование, след, ранг, определитель и инверсия матрицы

Для выполнения таких операций над матрицами, как транспонирование, диагонализация, определение следа, ранга, определителя матрицы и т.п. можно воспользоваться библиотекой (пакетом) LinearAlgebra.

![Ранг, инверсия, определитель, псевдобратная](image/5.png){ #fig:005 width=50% }

## Вычисление нормы векторов и матриц, повороты, вращения

Вычисление евклидовой нормы и p-нормы для векторов.

![Нормы для векторов](image/6.png){ #fig:006 width=50% }

## Вычисление нормы векторов и матриц, повороты, вращения

Вычисление нормы для двумерной матрицы.

![Нормы для матрицы](image/8.png){ #fig:008 width=50% }

## Матричное умножение, единичная матрица, скалярное произведение

Произведение матриц A и B:

![Произведение](image/10.png){ #fig:010 width=50% }

## Матричное умножение, единичная матрица, скалярное произведение

Скалярное произведение векторов X и Y:

![Скалярное произведение](image/11.png){ #fig:011 width=50% }

## Факторизация. Специальные матричные структуры

Решение систем линейный алгебраических уравнений 𝐴𝑥 = 𝑏:

![Ax = b](image/12.png){ #fig:012 width=50% }

## Факторизация. Специальные матричные структуры

Julia позволяет вычислять LU-факторизацию и определяет составной тип факторизации для его хранения.

Julia позволяет вычислять QR-факторизацию и определяет составной тип факторизации для его хранения.

## Факторизация. Специальные матричные структуры

Исходная система уравнений 𝐴𝑥 = 𝑏 может быть решена или с использованием исходной матрицы, или с использованием объекта факторизации:

![СЛАУ](image/14.png){ #fig:014 width=50% }

## Общая линейная алгебра

В следующем примере показано, как можно решить систему линейных уравнений с рациональными элементами без преобразования в типы элементов с плавающей запятой (для избежания проблемы с переполнением используем BigInt).

## Задание для самостаятельной работы

Произведение векторов. Задание 1.1 - 1.2

![Задание 1.1 - 1.2](image/24.png){ #fig:024 width=50% }

## Задание для самостаятельной работы

Системы линейных уравнений. Допустим пример Задание 2.1.f

![Задание 2.1.f](image/26.png){ #fig:026 width=60% }

## Задание для самостаятельной работы

Операции с матрицами. Задание 3.1.a - 3.1.c

![Задание 3.1.a - 3.1.c](image/28.png){ #fig:028 width=50% }

## Задание для самостаятельной работы

Операции с матрицами. Задание 3.2.a - 3.2.d

![Задание 3.2.a - 3.2.d](image/29.png){ #fig:029 width=50% }

## Задание для самостаятельной работы

Операции с матрицами. Задание 3.3 

![Задание 3.3](image/30.png){ #fig:030 width=50% }

## Задание для самостаятельной работы

Линейные модели экономики. Приведу один пример, остальные в отчете. Задание 4.2 

![Задание 4.2](image/32.png){ #fig:032 width=50% }

# Вывод

Изучила возможности специализированных пакетов Julia для выполнения и оценки эффективности операций над объектами линейной алгебры.