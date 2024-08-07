---
title: Lists to dictionary
type: snippet
language: python
tags: [list,dictionary]
excerpt: Combines two lists into a dictionary, using the first one as the keys and the second one as the values.
cover: purple-sunset
listed: true
dateModified: 2020-11-02
---

Combines two lists into a dictionary, where the elements of the first one serve as the keys and the elements of the second one serve as the values.
The values of the first list need to be unique and hashable.

- Use `zip()` in combination with `dict()` to combine the values of the two lists into a dictionary.

```py
def to_dictionary(keys, values):
  return dict(zip(keys, values))

to_dictionary(['a', 'b'], [1, 2]) # { a: 1, b: 2 }
```
