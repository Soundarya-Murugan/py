---
title: Retrieve-Multiple-Attributes
date: 2024-11-30
author: Your Name
cell_count: 5
score: 5
---

```python
import magicattr
```


```python
class Example:
    def __init__(self):
        self.name = 'example'
        self.version = 1.0
        self.description = 'A test example'
```


```python
# Create an instance of Example
obj = Example()
```


```python
# Accessing multiple attributes
attrs = [magicattr.get(obj, attr) for attr in ['name', 'version', 'description']]
print(attrs)  # Output: ['example', 1.0, 'A test example']
```

    ['example', 1.0, 'A test example']



```python

```


---
**Score: 5**
