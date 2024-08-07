---
title: Spread list
type: snippet
language: python
tags: [list]
cover: digital-nomad-14
excerpt: Flattens a list, by spreading its elements into a new list.
listed: true
dateModified: 2020-09-15
---

Flattens a list, by spreading its elements into a new list.

- Loop over elements, use `list.extend()` if the element is a list, `list.append()` otherwise.

```py
def spread(arg):
  ret = []
  for i in arg:
    ret.extend(i) if isinstance(i, list) else ret.append(i)
  return ret

spread([1, 2, 3, [4, 5, 6], [7], 8, 9]) # [1, 2, 3, 4, 5, 6, 7, 8, 9]
```
