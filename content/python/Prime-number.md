---
title: Prime-Number
date: 2024-11-23
author: Your Name
cell_count: 3
score: 0
---

```python
# Function to check if a number is prime
def is_prime(num):
    if num <= 1:
        return False
    for i in range(2, int(num**0.5) + 1):
        if num % i == 0:
            return False
    return True




```


```python
# Test the function
number = 29
if is_prime(number):
    print(f"{number} is a prime number.")
else:
    print(f"{number} is not a prime number.")
```

    29 is a prime number.



```python

```


---
**Score: 0**
