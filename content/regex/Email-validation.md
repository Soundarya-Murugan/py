---
title: Email-Validation
date: 2024-11-22
author: Your Name
cell_count: 4
score: 0
---

```python
import re

```


```python
def validate_email(email):
    pattern = r'^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$'
if re.match(pattern, email):
        return True
    else:
        return False

```


```python

email = input("Enter email: ")
if validate_email(email):
    print("Valid email")
else:
    print("Invalid email")
```

    Enter email:  sound@gmail.com


    Invalid email



```python

```


---
**Score: 0**
