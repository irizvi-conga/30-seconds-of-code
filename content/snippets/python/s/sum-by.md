---
title: Sum list based on function
type: snippet
language: python
tags: [math,list]
cover: horse-sunset
excerpt: Calculates the sum of a list, after mapping each element to a value using the provided function.
listed: true
dateModified: 2020-11-02
---

Calculates the sum of a list, after mapping each element to a value using the provided function.

- Use `map()` with `fn` to map each element to a value using the provided function.
- Use `sum()` to return the sum of the values.

```py
def sum_by(lst, fn):
  return sum(map(fn, lst))

sum_by([{ 'n': 4 }, { 'n': 2 }, { 'n': 8 }, { 'n': 6 }], lambda v : v['n']) # 20
```
