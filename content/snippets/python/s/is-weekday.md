---
title: Date is weekday
type: snippet
language: python
tags: [date]
cover: succulent-4
excerpt: Checks if the given date is a weekday.
listed: true
dateModified: 2020-11-02
---

Checks if the given date is a weekday.

- Use `datetime.datetime.weekday()` to get the day of the week as an integer.
- Check if the day of the week is less than or equal to `4`.
- Omit the second argument, `d`, to use a default value of `datetime.today()`.

```py
from datetime import datetime, date

def is_weekday(d = datetime.today()):
  return d.weekday() <= 4

is_weekday(date(2020, 10, 25)) # False
is_weekday(date(2020, 10, 28)) # True
```
