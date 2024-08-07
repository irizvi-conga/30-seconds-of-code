---
title: Min list value based on function
type: snippet
language: python
tags: [math,list]
cover: purple-flower-field
excerpt: Returns the minimum value of a list, after mapping each element to a value using the provided function.
listed: true
dateModified: 2020-11-02
---

Returns the minimum value of a list, after mapping each element to a value using the provided function.

- Use `map()` with `fn` to map each element to a value using the provided function.
- Use `min()` to return the minimum value.

```py
def min_by(lst, fn):
  return min(map(fn, lst))

min_by([{ 'n': 4 }, { 'n': 2 }, { 'n': 8 }, { 'n': 6 }], lambda v : v['n']) # 2
```
