---
title: Find keys with value
type: snippet
language: python
tags: [dictionary]
cover: laptop-plants-2
excerpt: Finds all keys in the provided dictionary that have the given value.
listed: true
dateModified: 2020-11-02
---

Finds all keys in the provided dictionary that have the given value.

- Use `dictionary.items()`, a generator and `list()` to return all keys that have a value equal to `val`.

```py
def find_keys(dict, val):
  return list(key for key, value in dict.items() if value == val)

ages = {
  'Peter': 10,
  'Isabel': 11,
  'Anna': 10,
}
find_keys(ages, 10) # [ 'Peter', 'Anna' ]
```
