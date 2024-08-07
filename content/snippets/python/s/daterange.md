---
title: Date range
type: snippet
language: python
tags: [date]
cover: maple-leaf-palette
excerpt: Creates a list of dates between `start` (inclusive) and `end` (not inclusive).
listed: true
dateModified: 2021-01-07
---

Creates a list of dates between `start` (inclusive) and `end` (not inclusive).

- Use  `datetime.timedelta.days` to get the days between `start` and `end`.
- Use `int()` to convert the result to an integer and `range()` to iterate over each day.
- Use a list comprehension and `datetime.timedelta` to create a list of `datetime.date` objects.

```py
from datetime import timedelta, date

def daterange(start, end):
  return [start + timedelta(n) for n in range(int((end - start).days))]

daterange(date(2020, 10, 1), date(2020, 10, 5))
# [date(2020, 10, 1), date(2020, 10, 2), date(2020, 10, 3), date(2020, 10, 4)]
```
