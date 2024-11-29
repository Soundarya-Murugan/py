---
title: Generate-Condition-Ends
date: 2024-11-29
author: Your Name
cell_count: 5
score: 5
---

```python
import namegenerator


```


```python
def generate_until_condition(condition):
    while True:
        name = namegenerator.gen()
        if condition(name):
            return name



```


```python
# Example: Generate a name with more than 6 characters
name = generate_until_condition(lambda x: len(x) > 6)

```


```python
print(name)
```

    cozy-cerise-mule



```python

```


---
**Score: 5**
