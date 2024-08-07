---
title: Check property
type: snippet
language: python
tags: [function]
cover: lake-trees
excerpt: Creates a function that will invoke a predicate function for the specified property on a given dictionary.
listed: true
dateModified: 2020-11-02
---

Creates a function that will invoke a predicate function for the specified property on a given dictionary.

- Return a `lambda` function that takes a dictionary and applies the predicate function, `fn` to the specified property.

```py
def check_prop(fn, prop):
  return lambda obj: fn(obj[prop])

check_age = check_prop(lambda x: x >= 18, 'age')
user = {'name': 'Mark', 'age': 18}
check_age(user) # True
```
