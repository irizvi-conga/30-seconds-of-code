---
title: Capitalize every word
type: snippet
language: python
tags: [string]
cover: trippy-chemicals
excerpt: Capitalizes the first letter of every word in a string.
listed: true
dateModified: 2020-11-02
---

Capitalizes the first letter of every word in a string.

- Use `str.title()` to capitalize the first letter of every word in the string.

```py
def capitalize_every_word(s):
  return s.title()

capitalize_every_word('hello world!') # 'Hello World!'
```
