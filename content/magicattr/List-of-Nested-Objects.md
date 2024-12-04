---
title: List-Of-Nested-Objects
date: 2024-12-04
author: Your Name
cell_count: 7
score: 5
---

```python
import magicattr

```


```python
class SubExample:
    def __init__(self, c):
        self.c = c


```


```python

class Example:
    def __init__(self):
        self.a = [SubExample(1), SubExample(2), SubExample(3)]



```


```python
obj = Example()


```


```python
# Use list comprehension to access the attribute 'c' in each object in the list 'a'
c_values = [magicattr.get(item, 'c') for item in obj.a]

```


```python
print(c_values)  # Output: [1, 2, 3]
```

    [1, 2, 3]



```python

```


---
**Score: 5**
