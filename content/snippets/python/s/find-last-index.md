---
title: Find last matching index
type: snippet
language: python
tags: [list]
cover: succulent-8
excerpt: Finds the index of the last element in the given list that satisfies the provided testing function.
listed: true
dateModified: 2020-11-02
---

Finds the index of the last element in the given list that satisfies the provided testing function.

- Use a list comprehension, `enumerate()` and `next()` to return the index of the last element in `lst` for which `fn` returns `True`.

```py
def find_last_index(lst, fn):
  return len(lst) - 1 - next(i for i, x in enumerate(lst[::-1]) if fn(x))

find_last_index([1, 2, 3, 4], lambda n: n % 2 == 1) # 2
```
