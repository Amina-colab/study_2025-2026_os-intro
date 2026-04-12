---
## Author
author:
  name: Юсупова Амина Руслановна
  affiliation:
    - name: Российский университет дружбы народов
      country: Российская Федерация
      postal-code: 117198
      city: Москва
      address: ул. Миклухо-Маклая, д. 6
lang: ru
format:
  pdf:
    documentclass: scrartcl
    latex-engine: xelatex
    mainfont: "Liberation Serif"
    sansfont: "Liberation Sans"
    monofont: "Liberation Mono"
    include-in-header:
      text: |
        \usepackage{fontspec}
        \setmainfont{Liberation Serif}
        \setsansfont{Liberation Sans}
        \setmonofont{Liberation Mono}
  pptx:
    toc: false
## Title
title: Лабораторная работа №10
subtitle: Текстовой редактор vi
license: CC BY

---

# Цели и задачи лабораторной работы

## Цель работы

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором vi, установленным по умолчанию практически во всех дистрибутивах.

# Выполнение лабораторной работы

## Задание 1. Создание нового файла с использованием vi

![Ввод команды](./image/02.png){#fig:001 width=70%}

##

Файл сделан исполняемым: chmod +x hello.sh.

![Исполняемый файл](./image/03.png){#fig:002 width=70%}

## Задание 2. Редактирование существующего файла

![Редактирование файла](./image/04.png){#fig:003 width=70%}

# Выводы по проделанной работе 

## Выводы 

В ходе лабораторной работы я познакомилась с операционной системой Linux и получила практические навыки работы с редактором vi. Были освоены: создание новых файлов с помощью vi; переход между режимами (командный, вставки, последней строки); удаление символов, слов и строк; отмена действий с помощью команды u; сохранение изменений и выход из редактора.

