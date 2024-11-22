---
title: Handle-Missing-Attributes
date: 2024-11-22
author: Your Name
cell_count: 5
score: 5
---

```python
import magicattr

```


```python
class Example:
    pass
```


```python

obj = Example()

```


```python
print(magicattr.get(obj, 'a.b.c', default='default_value'))  # Output: 'default_value'
```

    default_value



```python

```


---
**Score: 5**
