---
title: Fibonacci-Series
date: 2024-11-23
author: Your Name
cell_count: 4
score: 0
---

```python
# Function to generate Fibonacci sequence
def fibonacci(n):
    sequence = []
    a, b = 0, 1
    for _ in range(n):
        sequence.append(a)
        a, b = b, a + b
    return sequence


```


```python
# Number of terms to generate
terms = 10


```


```python
print(f"Fibonacci sequence with {terms} terms: {fibonacci(terms)}")
```

    Fibonacci sequence with 10 terms: [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]



```python

```


---
**Score: 0**
