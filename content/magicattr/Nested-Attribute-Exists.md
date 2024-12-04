---
title: Nested-Attribute-Exists
date: 2024-12-04
author: Your Name
cell_count: 6
score: 5
---

```python
import magicattr

```


```python

def has_attr(obj, attr):
    try:
        magicattr.get(obj, attr)
        return True
    except AttributeError:
        return False



```


```python
class Example:
    def __init__(self):
        self.a = {'b': {'c': 'value'}}


```


```python
obj = Example()


```


```python
# Check if nested attributes exist
print(has_attr(obj, 'a.b.c'))  # Output: True
print(has_attr(obj, 'a.b.d'))  # Output: False
```

    False
    False



```python

```


---
**Score: 5**
