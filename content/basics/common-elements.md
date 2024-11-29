---
title: Common-Elements
date: 2024-11-30
author: Your Name
cell_count: 3
score: 0
---

```python
def find_common_elements(list1, list2):
    """
    Given two lists, find the common elements between them.

    Args:
    list1: First list of elements
    list2: Second list of elements

    Returns:
    List of common elements between list1 and list2
    """

    # Initialize an empty list to store common elements
    common_elements = []

    for element in list1:
        if element in list2:
            if element not in common_elements:
                common_elements.append(element)

    return common_elements    
    
# Sample test cases
# print(find_common_elements([1, 2, 3, 4, 5], [4, 5, 6, 7, 8])) # Output should be [4, 5]
# print(find_common_elements(['a', 'b', 'c'], ['b', 'c', 'd'])) # Output should be ['b', 'c']

```


```python
print(find_common_elements([1, 2, 3, 4, 5], [4, 5, 6, 7, 8]))
```

    [4, 5]



```python

```


---
**Score: 0**
