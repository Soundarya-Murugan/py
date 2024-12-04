---
title: Web-Color-String
date: 2024-12-04
author: Your Name
cell_count: 7
score: 5
---

```python
import webcolors
```


```python
#Webcolors using by string it will return that hex color code is true or flas
```


```python
def is_valid_hex_color(color):
    try:
        webcolors.hex_to_rgb(color)
        return True
    except Exception as e:
        return False
```


```python
# Examples
print(is_valid_hex_color("#FFF"))  # True
```

    True



```python
print(is_valid_hex_color("#123ABC"))  # True
```

    True



```python
print(is_valid_hex_color("#123ABCG"))  # False
```

    False



```python

```


---
**Score: 5**
