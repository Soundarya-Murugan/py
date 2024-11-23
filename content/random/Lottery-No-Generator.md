---
title: Lottery-No-Generator
date: 2024-11-23
author: Your Name
cell_count: 5
score: 5
---

```python
#Lottery Number Generator
```


```python
import random
```


```python
def generate_lottery_numbers():
    main_numbers = random.sample(range(1, 50), 5)
    powerball = random.randint(1, 20)
    return main_numbers, powerball
```


```python
print("Lottery Numbers:")
for i in range(3):
    main, powerball = generate_lottery_numbers()
    print(f"Main Numbers: {main}, Powerball: {powerball}")

```

    Lottery Numbers:
    Main Numbers: [7, 48, 33, 18, 1], Powerball: 2
    Main Numbers: [13, 43, 5, 26, 17], Powerball: 14
    Main Numbers: [41, 26, 32, 21, 46], Powerball: 10



```python

```


---
**Score: 5**
