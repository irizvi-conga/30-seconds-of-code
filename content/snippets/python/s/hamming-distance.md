---
title: Hamming distance
type: snippet
language: python
tags: [math]
cover: tulips-and-reeds
excerpt: Calculates the Hamming distance between two values.
listed: true
dateModified: 2021-02-18
---

Calculates the Hamming distance between two values.

- Use the XOR operator (`^`) to find the bit difference between the two numbers.
- Use `bin()` to convert the result to a binary string.
- Convert the string to a list and use `count()` of `str` class to count and return the number of `1`s in it.

```py
def hamming_distance(a, b):
  return bin(a ^ b).count('1')

hamming_distance(2, 3) # 1
```
