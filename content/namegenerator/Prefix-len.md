---
title: Prefix-Len
date: 2024-11-23
author: Your Name
cell_count: 7
score: 5
---

```python
import namegenerator



```


```python
def generate_names_with_prefix(prefix, min_length):
    name = namegenerator.gen(prefix)
    while len(name) < min_length:
        name = namegenerator.gen(prefix)
    return name


```


```python
prefix = "super"

```


```python
min_length = 8

```


```python
name = generate_names_with_prefix(prefix, min_length)

```


```python
print(f"Generated name: {name}")
```

    Generated name: stuffy-wheat-harrier



```python

```


---
**Score: 5**
