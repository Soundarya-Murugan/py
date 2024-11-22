---
title: Set-Attributes-Nested
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

# Manually set the 'c' attribute in each item of the list
for sub in obj.a:
    magicattr.set(sub, 'c', 10)

# Print updated 'c' values
print([sub.c for sub in obj.a])  # Output: [10, 10, 10]


```

    [10, 10, 10]



```python

```


---
**Score: 0**
