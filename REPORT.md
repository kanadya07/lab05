# Отчет по лабораторной работе №5

## Тема работы

Изучение средств модульного тестирования.

## Цель работы

Познакомиться с тестами и оформить домашнее задание для библиотеки `banking`.

## Ход работы

### 1. Подготовка проекта

Сначала я взяла проект из лабораторной работы №4 и на его основе создала новый
репозиторий `lab05`.

Команды:

```bash
git clone https://github.com/kanadya07/lab04.git lab05
cd lab05
git remote remove origin
git remote add origin https://github.com/kanadya07/lab05.git
```

### 2. Добавление библиотеки banking

Дальше по домашнему заданию я добавила папку `banking`, в которой находятся
классы `Account` и `Transaction`.

```bash
mkdir banking
touch banking/Account.h
touch banking/Account.cpp
touch banking/Transaction.h
touch banking/Transaction.cpp
touch banking/CMakeLists.txt
```

### 3. Добавление тестов

После этого я создала папку `tests` и добавила туда тесты.

```bash
mkdir tests
touch tests/account_test.cpp
touch tests/transaction_test.cpp
```

### 4. Настройка сборки

Потом в основной `CMakeLists.txt` я добавила подключение тестов и библиотеки
`banking`.

После этого проект можно собирать и запускать тесты такими командами:

```bash
cmake -S . -B _build
cmake --build _build
ctest --test-dir _build --output-on-failure
```

### 5. Оформление репозитория

В конце я добавила задание и отчет.

```bash
git add TASK.md REPORT.md
git commit -m "Добавила задание и отчет"
git push origin master
```

## Что находится в репозитории

1. `TASK.md`
2. `REPORT.md`
3. `banking`
4. `tests`
5. проект из предыдущих лабораторных работ

## Вывод

Во время выполнения этой лабораторной работы я познакомилась с тестами и
увидела, что с их помощью можно проверять работу классов и методов.

## Ссылка на репозиторий

https://github.com/kanadya07/lab05
