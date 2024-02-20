---
hide:
  - feedback
title: Тестовый пост
author: Artyom Semenov
date: 2024-02-20
---

## Это текстовый блок чтобы показать, что в целом можно сделать с текстом.

Text can be {--deleted--} and replacement text {++added++}. This can also be
combined into {~~one~>a single~~} operation. {==Highlighting==} is also
possible {>>and comments can be added inline<<}.

{==

Formatting can also be applied to blocks by putting the opening and closing
tags on separate lines and adding new lines between the tags and the content.

==}

## Как будет выглядть код

``` py title="bubble_sort.py"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```


``` py title="bubble_sort.py" linenums="1"
def bubble_sort(items):
    for i in range(len(items)):
        for j in range(len(items) - 1 - i):
            if items[j] > items[j + 1]:
                items[j], items[j + 1] = items[j + 1], items[j]
```
## Нажимаем клавиши

++ctrl+alt+del++

## Пишем формулы

- H~2~O
- A^T^A

[^1]:
    А вот тут мы тестируем FootNotes. Можно их к примеру оставлять в постах где есть *