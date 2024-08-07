---
title: Check if list has no duplicates
type: snippet
language: python
tags: [list]
cover: touch-flower
excerpt: Checks if all the values in a list are unique.
listed: true
dateModified: 2021-01-07
---

Checks if all the values in a list are unique.

- Use `set()` on the given list to keep only unique occurrences.
- Use `len()` to compare the length of the unique values to the original list.

```py
def all_unique(lst):
  return len(lst) == len(set(lst))

x = [1, 2, 3, 4, 5, 6]
y = [1, 2, 2, 3, 4, 5]
all_unique(x) # True
all_unique(y) # False
```
