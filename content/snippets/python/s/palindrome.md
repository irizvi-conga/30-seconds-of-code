---
title: Palindrome
type: snippet
language: python
tags: [string]
cover: succulent-6
excerpt: Checks if the given string is a palindrome.
listed: true
dateModified: 2020-11-02
---

Checks if the given string is a palindrome.

- Use `str.lower()` and `re.sub()` to convert to lowercase and remove non-alphanumeric characters from the given string.
- Then, compare the new string with its reverse, using slice notation.

```py
from re import sub

def palindrome(s):
  s = sub('[\W_]', '', s.lower())
  return s == s[::-1]

palindrome('taco cat') # True
```
