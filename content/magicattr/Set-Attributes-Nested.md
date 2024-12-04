---
title: Set-Attributes-Nested
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
# Manually set the 'c' attribute in each item of the list
for sub in obj.a:
    magicattr.set(sub, 'c', 10)


```


```python
# Print updated 'c' values
print([sub.c for sub in obj.a])  # Output: [10, 10, 10]
```

    [10, 10, 10]



```python

```


---
**Score: 5**
