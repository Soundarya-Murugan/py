---
title: Nested-Attribute-Exists
date: 2024-11-22
author: Your Name
cell_count: 2
score: 0
---

```python
import magicattr

def has_attr(obj, attr):
    try:
        magicattr.get(obj, attr)
        return True
    except AttributeError:
        return False

class Example:
    def __init__(self):
        self.a = {'b': {'c': 'value'}}

obj = Example()

# Check if nested attributes exist
print(has_attr(obj, 'a.b.c'))  # Output: True
print(has_attr(obj, 'a.b.d'))  # Output: False

```

    False
    False



```python

```


---
**Score: 0**
