---
title: Add-Timestamp
date: 2024-11-22
author: Your Name
cell_count: 6
score: 5
---

```python
import namegenerator

```


```python
from datetime import datetime



```


```python
def generate_name_with_timestamp():
    name = namegenerator.gen()
    timestamp = datetime.now().strftime("%Y%m%d%H%M%S")
    return f"{name}_{timestamp}"


```


```python
generated_name = generate_name_with_timestamp()

```


```python
print(f"Generated name with timestamp: {generated_name}")
```

    Generated name with timestamp: dorky-myrtle-collie_20241122230315



```python

```


---
**Score: 5**
