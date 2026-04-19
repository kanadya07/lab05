# REPORT

## Laboratory work V

В репозитории выполнена лабораторная работа по GTest/GMock и домашняя работа по библиотеке `banking`.

## Что сделано

1. Перенесен проект из `lab04`.
2. Добавлена библиотека `banking`.
3. Добавлен `CMakeLists.txt` для `banking`.
4. Подключены `GTest` и `GMock` через `FetchContent`.
5. Написаны тесты:
   - `tests/account_test.cpp`
   - `tests/transaction_test.cpp`
6. В репозиторий добавлены `TASK.md` и `REPORT.md`.

## Проверка

```bash
cmake -S . -B _build
cmake --build _build
ctest --test-dir _build --output-on-failure
```

## Ссылки

- Репозиторий: `https://github.com/kanadya07/lab05`
- Задание: `TASK.md`
