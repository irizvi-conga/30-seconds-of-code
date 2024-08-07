---
title: Check for duplicates in list
type: snippet
language: python
tags: [list]
cover: jars-on-shelf-2
excerpt: Checks if there are duplicate values in a flat list.
listed: true
dateModified: 2020-11-02
---

Checks if there are duplicate values in a flat list.

- Use `set()` on the given list to remove duplicates, compare its length with the length of the list.

```py
def has_duplicates(lst):
  return len(lst) != len(set(lst))

x = [1, 2, 3, 4, 5, 5]
y = [1, 2, 3, 4, 5]
has_duplicates(x) # True
has_duplicates(y) # False
```
