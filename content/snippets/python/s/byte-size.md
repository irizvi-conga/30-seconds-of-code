---
title: Byte size of string
type: snippet
language: python
tags: [string]
cover: river-house-lights
excerpt: Returns the length of a string in bytes.
listed: true
dateModified: 2020-11-02
---

Returns the length of a string in bytes.

- Use `str.encode()` to encode the given string and return its length.

```py
def byte_size(s):
  return len(s.encode('utf-8'))

byte_size('😀') # 4
byte_size('Hello World') # 11
```
