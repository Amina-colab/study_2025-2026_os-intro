---
marp: true
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
title: Лабораторная работа №4
subtitle: Продвинутое использование git
license: CC BY
---

# Цели и задачи работы

---
## Цель лабораторной работы

Получение навыков правильной работы с репозиториями git.
---
---
# Процесс выполнения лабораторной работы
---

## Установка Git Flow

Для управления ветками было установлено расширение Git Flow. Репозиторий Copr включён, пакет установлен.

![Установка Git Flow](./image/01.png){#fig:001 width=70% height=70%}

---
## Установка Node.js и pnpm

Node.js необходим для работы пакетного менеджера pnpm, который используется для установки Commitizen. После установки выполнена настройка окружения.

![Установка Node.js](./image/02.png){#fig:002 width=70% height=70%}
---
---

![Установка pnpm](./image/03.png){#fig:003 width=70% height=70%}

---
![Настройка pnpm](./image/04.png){#fig:004 width=70% height=70%}

---

## Создание репозитория и первый push

Создан локальный репозиторий `git-extended`, добавлен файл `README.md`, выполнена привязка к удалённому репозиторию на GitHub и произведён первый push.

![Связь с GitHub](./image/06.png){#fig:006 width=70% height=70%}

---

## Инициализация Git Flow

С помощью команды `git flow init` созданы основные ветки `master` и `develop` с параметрами по умолчанию.

![Инициализация Git Flow](./image/07.png){#fig:007 width=70% height=70%}

---
## Отправка ветки develop

Ветка `develop` отправлена на сервер и настроена на отслеживание удалённой ветки.

![Отправка develop](./image/08.png){#fig:008 width=70% height=70%}

---

## Настройка package.json и Commitizen

Создан файл `package.json` через `pnpm init`, отредактирован: добавлено описание, автор, лицензия, настроен Commitizen для конвенциональных коммитов.

![Редактирование package.json](./image/09.png){#fig:009 width=70% height=70%}

---

Коммит выполнен с помощью `git cz`, что обеспечило соблюдение стандарта Conventional Commits.

![Коммит через git cz](./image/10.png){#fig:010 width=70% height=70%}

---

## Создание первого релиза (v1.0.0)

Создана релизная ветка, сгенерирован `CHANGELOG.md` с помощью `standard-changelog`. Релиз завершён, тег создан вручную из-за ошибки автоматического создания.

![Генерация changelog](./image/11.png){#fig:011 width=70% height=70%}

---

![Завершение релиза и создание тега](./image/12.png){#fig:012 width=70% height=70%}

---

Ветки и теги отправлены на GitHub, релиз опубликован через `gh release create`.

![Публикация релиза](./image/13.png){#fig:013 width=70% height=70%}

---

## Работа с feature-веткой

Создана feature-ветка, в неё добавлен файл `example.txt`, сделан коммит через `git cz`. После завершения ветка слита в `develop`.

![Создание feature-ветки](./image/14.png){#fig:014 width=70% height=70%}

---

## Создание второго релиза (v1.2.3)

Аналогично первому релизу создана ветка `release/1.2.3`, обновлён `CHANGELOG.md`. При завершении снова возникла ошибка с тегом, но слияние прошло успешно. Релиз создан на GitHub.

![Подготовка второго релиза](./image/15.png){#fig:015 width=70% height=70%}

---

![Публикация второго релиза](./image/16.png){#fig:016 width=70% height=70%}

---

# Выводы по проделанной работе

---

## Вывод

В ходе выполнения лабораторной работы были освоены основные приёмы работы с Git Flow:

- установка и настройка инструментов (Git Flow, Node.js, pnpm, Commitizen);
- инициализация репозитория с ветками `master` и `develop`;
- создание и завершение feature-веток;
- подготовка и публикация релизов с автоматической генерацией changelog;
- использование конвенциональных коммитов через Commitizen.

