---
title: Generate-Names-Len
date: 2024-11-27
author: Your Name
cell_count: 4
score: 0
---

```python
import namegenerator


```


```python
def generate_names(length):
    name = namegenerator.gen()
    while len(name) < length:
        name = namegenerator.gen()
    return name



```


```python

name = generate_names(10)
print(name)
```

    stinky-ruby-maltese



```python

```


---
**Score: 0**
