---
title: Retrieve-Multiple-Attributes
date: 2024-11-22
author: Your Name
cell_count: 2
score: 0
---

```python
import magicattr

class Example:
    def __init__(self):
        self.name = 'example'
        self.version = 1.0
        self.description = 'A test example'

# Create an instance of Example
obj = Example()

# Accessing multiple attributes
attrs = [magicattr.get(obj, attr) for attr in ['name', 'version', 'description']]
print(attrs)  # Output: ['example', 1.0, 'A test example']

```

    ['example', 1.0, 'A test example']



```python

```


---
**Score: 0**
