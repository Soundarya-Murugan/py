---
title: Access-Modify-Deeply-Nested
date: 2024-12-04
author: Your Name
cell_count: 8
score: 5
---

```python
import magicattr

```


```python
# Define the Inner class
class Inner:
    def __init__(self):
        self.value = 5

```


```python

# Define the Outer class
class Outer:
    def __init__(self):
        self.inner = Inner()

```


```python
# Create an instance of Outer
obj = Outer()

```


```python
# Accessing the nested attribute 'value' using magicattr
print(magicattr.get(obj, 'inner.value'))  # Output: 5
```

    5



```python

# Setting the nested attribute 'value' using magicattr
magicattr.set(obj, 'inner.value', 10)

```


```python
# Verify the update
print(obj.inner.value)  # Output: 10
```

    10



```python

```


---
**Score: 5**
