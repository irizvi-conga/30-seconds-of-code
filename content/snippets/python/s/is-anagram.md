---
title: String is anagram
type: snippet
language: python
tags: [string]
cover: digital-nomad-8
excerpt: Checks if a string is an anagram of another string (case-insensitive, ignores spaces, punctuation and special characters).
listed: true
dateModified: 2020-11-02
---

Checks if a string is an anagram of another string (case-insensitive, ignores spaces, punctuation and special characters).

- Use `str.isalnum()` to filter out non-alphanumeric characters, `str.lower()` to transform each character to lowercase.
- Use `collections.Counter` to count the resulting characters for each string and compare the results.

```py
from collections import Counter

def is_anagram(s1, s2):
  return Counter(
    c.lower() for c in s1 if c.isalnum()
  ) == Counter(
    c.lower() for c in s2 if c.isalnum()
  )

is_anagram('#anagram', 'Nag a ram!')  # True
```
