---
title: Find key of value
type: snippet
language: python
tags: [dictionary]
cover: blue-red-mountain
excerpt: Finds the first key in the provided dictionary that has the given value.
listed: true
dateModified: 2020-11-02
---

Finds the first key in the provided dictionary that has the given value.

- Use `dictionary.items()` and `next()` to return the first key that has a value equal to `val`.

```py
def find_key(dict, val):
  return next(key for key, value in dict.items() if value == val)

ages = {
  'Peter': 10,
  'Isabel': 11,
  'Anna': 9,
}
find_key(ages, 11) # 'Isabel'
```
