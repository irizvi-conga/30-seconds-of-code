---
title: Merge dictionaries
type: snippet
language: python
tags: [dictionary]
cover: plant-candle
excerpt: Merges two or more dictionaries.
listed: true
dateModified: 2020-11-02
---

Merges two or more dictionaries.

- Create a new `dict` and loop over `dicts`, using `dictionary.update()` to add the key-value pairs from each one to the result.

```py
def merge_dictionaries(*dicts):
  res = dict()
  for d in dicts:
    res.update(d)
  return res

ages_one = {
  'Peter': 10,
  'Isabel': 11,
}
ages_two = {
  'Anna': 9
}
merge_dictionaries(ages_one, ages_two)
# { 'Peter': 10, 'Isabel': 11, 'Anna': 9 }
```
