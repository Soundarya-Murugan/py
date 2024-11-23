---
title: Email-Validation
date: 2024-11-23
author: Your Name
cell_count: 6
score: 5
---

```python
#Validates if a given email address meets common email standards.
```


```python
import re


```


```python
def is_valid_email(email):
    # Regular expression for validating an email
    email_regex = r'^[a-zA-Z0-9_.+-]+@[a-zA-Z0-9-]+\.[a-zA-Z0-9-.]+$'
    return bool(re.match(email_regex, email))


```


```python
# Test cases
emails = [
    "test@example.com",
    "user.name+tag+sorting@example.com",
    "user@sub.example.com",
    "invalid-email",
    "@missinguser.com",
    "user@.com"
]



```


```python
for email in emails:
    print(f"{email}: {'Valid' if is_valid_email(email) else 'Invalid'}")
```

    test@example.com: Valid
    user.name+tag+sorting@example.com: Valid
    user@sub.example.com: Valid
    invalid-email: Invalid
    @missinguser.com: Invalid
    user@.com: Invalid



```python

```


---
**Score: 5**
