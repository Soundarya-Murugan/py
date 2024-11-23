---
title: Multiple-Names
date: 2024-11-23
author: Your Name
cell_count: 5
score: 5
---

```python
import namegenerator


```


```python
def generate_unique_names(num):
    unique_names = set()
    while len(unique_names) < num:
        name = namegenerator.gen()
        if name not in unique_names:
            unique_names.add(name)
    return list(unique_names)
names = generate_unique_names(5)
print("Generated unique names:")
for name in names:
    print(name)

```

    Generated unique names:
    gimpy-coral-bombay
    leaky-firebrick-tang
    frumpy-saffron-mayfly
    gloppy-lilac-caiman
    dorky-scarlet-horse



```python

```


```python

```


```python

```


---
**Score: 5**
