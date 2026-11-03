# Tagged-Nullity Arithmetic (⊥)

**A non-contradictory system for division by zero with recoverable dividends.**

Автор / Author: **Alexey Dmitriyev** (Lex474.by@gmail.com)
Лицензия / License: **CC BY 4.0** (text, concept) + **MIT** (code)
Публикация / Publication: **DOI 10.5281/zenodo.23884948** (latest version / всегда актуальная)


## What is this / Что это

В стандартной арифметике деление на ноль уничтожает данные: `x / 0` даёт NaN
или исключение, и делимое теряется навсегда. Здесь результат размечается:
`x / 0 = ⊥(x)` — метка несёт делимое в себе. Восстановление выполняет
отдельная операция `extract(⊥(x)) = x`, которая **не участвует в умножении**
— это защита от коллапса системы (теорема: если бы восстановление было
умножением на ноль, ассоциативность дала бы 2 = 1).

In standard arithmetic, division by zero destroys data: `x / 0` yields NaN
or an exception, and the dividend is lost forever. Here the result is tagged:
`x / 0 = ⊥(x)` — the tag carries the dividend. Recovery is a separate
operation `extract(⊥(x)) = x` that does **not** participate in
multiplication — this protects the system from collapse (theorem: if
recovery were multiplication by zero, associativity would yield 2 = 1).

## Files / Файлы

| Файл | Содержание |
|---|---|
| `PAPER.md` / `PAPER.pdf` | Статья (English): определения, теорема о коллапсе, связь с wheel theory и meadows |
| `tagged_nullity.py` | Референс-реализация на Python с тестами: `python3 tagged_nullity.py` |
| `LICENSE.txt` | CC BY 4.0 (текст/концепция) + MIT (код) |

## Related work / Связанная работа

Part 2 in preparation. / Вторая часть в подготовке.


## Citation / Цитирование

    Dmitriyev, A. (2026). Tagged-Nullity Arithmetic: A Non-Contradictory
    System for Division by Zero. Zenodo. https://doi.org/10.5281/zenodo.23884948
