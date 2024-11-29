---
title: Palindromatic-Names
date: 2024-11-29
author: Your Name
cell_count: 5
score: 5
---

```python
import namegenerator

```


```python

def check_if_palindromic(name):
    return name == name[::-1]



```


```python
name = namegenerator.gen()

```


```python
is_palindrome = check_if_palindromic(name)
print(f"Generated name: {name}")
print(f"Is palindrome: {is_palindrome}")
```

    Generated name: crabby-gold-tamarin
    Is palindrome: False



```python

```


---
**Score: 5**
