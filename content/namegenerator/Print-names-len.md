---
title: Print-Names-Len
date: 2024-11-23
author: Your Name
cell_count: 3
score: 0
---

```python
import namegenerator



```


```python
def validate_name_length(length):
    name = namegenerator.gen()
    if len(name) == length:
        print(f"Valid name of length {length}: {name}")
    else:
        print(f"Generated name does not meet the length requirement: {name}")


```


```python
validate_name_length(8)
```


---
**Score: 0**
