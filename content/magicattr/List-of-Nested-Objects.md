---
title: List-Of-Nested-Objects
date: 2024-11-22
author: Your Name
cell_count: 2
score: 0
---

```python
import magicattr

class SubExample:
    def __init__(self, c):
        self.c = c

class Example:
    def __init__(self):
        self.a = [SubExample(1), SubExample(2), SubExample(3)]

obj = Example()

# Use list comprehension to access the attribute 'c' in each object in the list 'a'
c_values = [magicattr.get(item, 'c') for item in obj.a]
print(c_values)  # Output: [1, 2, 3]

```

    [1, 2, 3]



```python

```


---
**Score: 0**
