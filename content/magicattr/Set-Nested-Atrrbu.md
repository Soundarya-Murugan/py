---
title: Set-Nested-Atrrbu
date: 2024-11-30
author: Your Name
cell_count: 6
score: 5
---

```python
import magicattr
```


```python
# Define the class
class Example:
    def __init__(self):
        self.a = {'b': {'c': 'value'}}  # a dictionary inside the object
```


```python
# Create an instance of Example
obj = Example()

```


```python
# Directly modify the dictionary attribute
obj.a['b']['c'] = 'new_value'

```


```python
# Output the modified value
print(obj.a['b']['c'])  # Expected Output: 'new_value'
```

    new_value



```python

```


---
**Score: 5**
