---
title: Reverse number
type: snippet
language: python
tags: [math]
cover: taking-photos
excerpt: Reverses a number.
listed: true
dateModified: 2020-11-02
---

Reverses a number.

- Use `str()` to convert the number to a string, slice notation to reverse it and `str.replace()` to remove the sign.
- Use `float()` to convert the result to a number and `math.copysign()` to copy the original sign.

```py
from math import copysign

def reverse_number(n):
  return copysign(float(str(n)[::-1].replace('-', '')), n)

reverse_number(981) # 189
reverse_number(-500) # -5
reverse_number(73.6) # 6.37
reverse_number(-5.23) # -32.5
```
