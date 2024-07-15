# Игры разума

[![Maintainability](https://api.codeclimate.com/v1/badges/1ccfac628567143c41d6/maintainability)](https://codeclimate.com/github/DaniillGolovin/php-project-lvl1/maintainability)
[![Github Actions Status](https://github.com/hexlet-boilerplates/php-package/workflows/PHP%20CI/badge.svg)](https://github.com/DaniillGolovin/php-project-lvl1/actions)

## Описание

> Проект **«Игры разума»** создан в рамках профессии **«Фронтенд-разработчик»** на платформе [Hexlet.io](https://ru.hexlet.io).

**«Игры разума»** — набор из пяти консольных игр, построенных по принципу популярных мобильных приложений для прокачки мозга. Каждая игра задает вопросы, на которые нужно дать правильные ответы. После трех правильных ответов считается, что игра пройдена. Неправильные ответы завершают игру и предлагают пройти ее заново.

### Игры

- [x] [Brain Even (определение четного числа)](#brain-even-определение-четного-числа)
- [x] [Brain Calc (калькулятор)](#brain-calc-калькулятор)
- [x] [Brain GCD (определение наибольшего общего делителя)](#brain-gcd-определение-наибольшего-общего-делителя)
- [x] [Brain Progression (арифметическая прогрессия)](#brain-progression-арифметическая-прогрессия)
- [x] [Brain Prime (определение простого числа)](#brain-prime-определение-простого-числа)

Команды, с помощью которых вызываются игры:

```bash
>> brain-even
>> braic-calc
>> brain-gcd
>> brain-progression
>> brain-prime
```

### Пример игры

```bash
$ brain-progression
Welcome to the Brain Game!
What number is missing in this progression?
May I have your name? Daniil
Hello, Daniil!
Question: 14 .. 18 20 22 24 26 28
>> Your answer: 16 # Пользователь вводит ответ
Correct!
Question: 5 6 7 8 9 .. 11 12
>> Your answer: 10 # Пользователь вводит ответ
Correct!
Question: 12 15 18 21 .. 27 30 33
>> Your answer: 24 # Пользователь вводит ответ
Correct!
Congratulations, Roman!
```

## Установка

```
⚠️ Перед установкой проекта проверьте наличие установленных php, composer!
```

Для запуска имеющихся игр необходимо предварительно установить данный проект:

1. Склонируйте репозиторий, используя одну из следующих консольных команд:

```bash
# HTTPS
>> git clone https://github.com/DaniillGolovin/Brain-Games.git
# SSH
>> git clone git@github.com:DaniillGolovin/Brain-Games.git
```

2. Осуществите установку проекта:

```bash
>> make install
```

3. Запустите любую из игр посредством команд, указанные [ниже](#превью).

Для глобальной установки выполните команду
```bash
>> composer global require daniillgolovin/php-project-lvl1
```

## Использование

### Превью

#### Brain Even (определение четного числа)

Команда для запуска: `brain-even`

[![asciicast](https://asciinema.org/a/JwqCgpJ7iGx4NaCYI4rOEwsGz.svg)](https://asciinema.org/a/JwqCgpJ7iGx4NaCYI4rOEwsGz)

#### Brain Calc (калькулятор)

Команда для запуска: `brain-calc`

[![asciicast](https://asciinema.org/a/iOib3cL3bITX5pUZQe9nluZwm.svg)](https://asciinema.org/a/iOib3cL3bITX5pUZQe9nluZwm)

#### Brain GCD (определение наибольшего общего делителя)

Команда для запуска: `brain-gcd`

[![asciicast](https://asciinema.org/a/qAW3HqT3XmaHwNChePww4E4AZ.svg)](https://asciinema.org/a/qAW3HqT3XmaHwNChePww4E4AZ)

#### Brain Progression (арифметическая прогрессия)

Команда для запуска: `brain-progression`

[![asciicast](https://asciinema.org/a/qed68AoUvNK856pM3R8b8JaNk.svg)](https://asciinema.org/a/qed68AoUvNK856pM3R8b8JaNk)

#### Brain Prime (определение простого числа)

Команда для запуска: `brain-prime`

[![asciicast](https://asciinema.org/a/6pQimP5KHKeRtNMCZEDwdui57.svg)](https://asciinema.org/a/6pQimP5KHKeRtNMCZEDwdui57)

## Структура проекта

```bash
.
└── Brain-Games
    ├── Makefile
    ├── README.md
    ├── bin
    │   ├── brain-calc
    │   ├── brain-even
    │   ├── brain-games
    │   ├── brain-gcd
    │   ├── brain-prime
    │   └── brain-progression
    ├── composer.json
    ├── composer.lock
    └── src
        ├── Cli.php
        ├── Engine.php
        └── Games
            ├── Calc.php
            ├── Even.php
            ├── Gcd.php
            ├── Prime.php
            └── Progression.php

4 directories, 17 files
```
