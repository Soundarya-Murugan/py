---
title: Date-Validator
date: 2024-11-30
author: Your Name
cell_count: 7
score: 5
---

```python
#Validates a date format (e.g., DD/MM/YYYY).
```


```python
import re


```


```python
def is_valid_date(date):
    date_regex = r'^(0[1-9]|[12][0-9]|3[01])/(0[1-9]|1[0-2])/\d{4}$'
    return bool(re.match(date_regex, date))

```


```python
# Test cases
dates = [
    "31/12/2020",
    "01/01/2000",
    "29/02/2021",
    "32/01/2021",
    "12/13/2021"
]

```


```python
#Print the date
```


```python

for date in dates:
    print(f"{date}: {'Valid' if is_valid_date(date) else 'Invalid'}")
```

    31/12/2020: Valid
    01/01/2000: Valid
    29/02/2021: Valid
    32/01/2021: Invalid
    12/13/2021: Invalid



```python

```


---
**Score: 5**
