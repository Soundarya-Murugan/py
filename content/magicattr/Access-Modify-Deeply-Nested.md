---
title: Access-Modify-Deeply-Nested
date: 2024-11-22
author: Your Name
cell_count: 2
score: 0
---

```python
import magicattr

# Define the Inner class
class Inner:
    def __init__(self):
        self.value = 5

# Define the Outer class
class Outer:
    def __init__(self):
        self.inner = Inner()

# Create an instance of Outer
obj = Outer()

# Accessing the nested attribute 'value' using magicattr
print(magicattr.get(obj, 'inner.value'))  # Output: 5

# Setting the nested attribute 'value' using magicattr
magicattr.set(obj, 'inner.value', 10)

# Verify the update
print(obj.inner.value)  # Output: 10

```

    5
    10



```python

```


---
**Score: 0**
