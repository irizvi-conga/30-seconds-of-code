---
title: N max elements
type: snippet
language: python
tags: [list,math]
cover: red-succulent
excerpt: Returns the `n` maximum elements from the provided list.
listed: true
dateModified: 2020-11-02
---

Returns the `n` maximum elements from the provided list.

- Use `sorted()` to sort the list.
- Use slice notation to get the specified number of elements.
- Omit the second argument, `n`, to get a one-element list.
- If `n` is greater than or equal to the provided list's length, then return the original list (sorted in descending order).

```py
def max_n(lst, n = 1):
  return sorted(lst, reverse = True)[:n]

max_n([1, 2, 3]) # [3]
max_n([1, 2, 3], 2) # [3, 2]
```
