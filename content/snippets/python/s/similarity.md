---
title: List similarity
type: snippet
language: python
tags: [list]
cover: sunflowers
excerpt: Returns a list of elements that exist in both lists.
listed: true
dateModified: 2020-11-02
---

Returns a list of elements that exist in both lists.

- Use a list comprehension on `a` to only keep values contained in both lists.

```py
def similarity(a, b):
  return [item for item in a if item in b]

similarity([1, 2, 3], [1, 2, 4]) # [1, 2]
```
