---
title: Username-Validator
date: 2024-11-30
author: Your Name
cell_count: 7
score: 5
---

```python
#Validates if a username meets specific criteria (e.g., length, characters).
```


```python
import re


```


```python
def is_valid_username(username):
    username_regex = r'^[a-zA-Z0-9_]{5,15}$'
    return bool(re.match(username_regex, username))

```


```python

# Test cases

```


```python
usernames = [
    "user_123",
    "a",
    "toolongusername123456",
    "valid_user",
    "invalid-user!"
]


```


```python
for username in usernames:
    print(f"{username}: {'Valid' if is_valid_username(username) else 'Invalid'}")
```

    user_123: Valid
    a: Invalid
    toolongusername123456: Invalid
    valid_user: Valid
    invalid-user!: Invalid



```python

```


---
**Score: 5**
