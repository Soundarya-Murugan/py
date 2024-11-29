---
title: Validate-Input
date: 2024-11-29
author: Your Name
cell_count: 5
score: 5
---

```python
import re



```


```python
def is_valid_ean13(ean):
    return bool(re.match(r'^\d{13}$', ean))


```


```python
ean_input = '123456789012'

```


```python
if is_valid_ean13(ean_input):
    print(f'{ean_input} is a valid EAN-13')
else:
    print(f'{ean_input} is not a valid EAN-13')
```

    123456789012 is not a valid EAN-13



```python

```


---
**Score: 5**
