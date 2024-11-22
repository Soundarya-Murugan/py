---
title: Set-Nested-Atrrbu
date: 2024-11-22
author: Your Name
cell_count: 2
score: 0
---

```python
import magicattr

# Define the class
class Example:
    def __init__(self):
        self.a = {'b': {'c': 'value'}}  # a dictionary inside the object

# Create an instance of Example
obj = Example()

# Directly modify the dictionary attribute
obj.a['b']['c'] = 'new_value'

# Output the modified value
print(obj.a['b']['c'])  # Expected Output: 'new_value'




```

    new_value



```python

```


---
**Score: 0**
