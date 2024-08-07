---
title: Least common multiple
type: snippet
language: python
tags: [math,list]
cover: chess-pawns
excerpt: Returns the least common multiple of a list of numbers.
listed: true
dateModified: 2020-11-02
---

Returns the least common multiple of a list of numbers.

- Use `functools.reduce()`, `math.gcd()` and `lcm(x, y) = x * y / gcd(x, y)` over the given list.

```py
from functools import reduce
from math import gcd

def lcm(numbers):
  return reduce((lambda x, y: int(x * y / gcd(x, y))), numbers)

lcm([12, 7]) # 84
lcm([1, 3, 4, 5]) # 60
```
