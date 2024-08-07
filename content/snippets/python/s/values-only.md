---
title: Dictionary values
type: snippet
language: python
tags: [dictionary,list]
cover: colorful-lounge
excerpt: Returns a flat list of all the values in a flat dictionary.
listed: true
dateModified: 2020-11-02
---

Returns a flat list of all the values in a flat dictionary.

- Use `dict.values()` to return the values in the given dictionary.
- Return a `list()` of the previous result.

```py
def values_only(flat_dict):
  return list(flat_dict.values())

ages = {
  'Peter': 10,
  'Isabel': 11,
  'Anna': 9,
}
values_only(ages) # [10, 11, 9]
```
