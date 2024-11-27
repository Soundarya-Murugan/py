---
title: Untitled
date: 2024-11-27
author: Your Name
cell_count: 3
score: 0
---

```python
def rotate_list(lst, k):
    """
    Rotate a list by k positions.

    Args:
    lst: list - the list to rotate
    k: int - the number of positions to rotate

    Returns:
    list - the rotated list
    """

    if not lst:
        return lst
    
    k = k % len(lst)  
    return lst[-k:] + lst[:-k]

# Sample test cases
# print(rotate_list([1, 2, 3, 4, 5], 2))  # Output: [4, 5, 1, 2, 3]
# print(rotate_list(['a', 'b', 'c', 'd', 'e'], 3))  # Output: ['c', 'd', 'e', 'a', 'b']
```


```python
print(rotate_list(['a', 'b', 'c', 'd', 'e'], 3))
```

    ['c', 'd', 'e', 'a', 'b']



```python

```


---
**Score: 0**
