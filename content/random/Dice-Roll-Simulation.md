---
title: Dice-Roll-Simulation
date: 2024-11-27
author: Your Name
cell_count: 9
score: 5
---

```python
#Dice Roll Simulation
```


```python
import random
```


```python
def roll_dice():
    return random.randint(1, 6)
```


```python
def simulate_dice_rolls(rolls=100):
    results = {i: 0 for i in range(1, 7)}
    for _ in range(rolls):
        roll = roll_dice()
        results[roll] += 1
    return results
```


```python
rolls = 1000
```


```python
results = simulate_dice_rolls(rolls)
```


```python
print(f"Dice Roll Simulation Results (Total Rolls: {rolls})")
```

    Dice Roll Simulation Results (Total Rolls: 1000)



```python
for num, count in results.items():
    print(f"{num}: {count}")

```

    1: 153
    2: 178
    3: 159
    4: 191
    5: 171
    6: 148



```python

```


---
**Score: 5**
