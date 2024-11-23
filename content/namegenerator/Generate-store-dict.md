---
title: Generate-Store-Dict
date: 2024-11-23
author: Your Name
cell_count: 9
score: 5
---

```python
import namegenerator



```


```python

```


```python
def store_names_in_dict(num):
    names_dict = {}
    for i in range(1, num+1):
        name = namegenerator.gen()
        names_dict[f"Name_{i}"] = name
    return names_dict


```


```python

```


```python
names_dict = store_names_in_dict(5)

```


```python
print("Generated names in dictionary:")
for key, value in names_dict.items():
    print(f"{key}: {value}")
```

    Generated names in dictionary:
    Name_1: squeaky-gamboge-fossa
    Name_2: goopy-plum-insect
    Name_3: silly-ochre-russel
    Name_4: breezy-fuchsia-falcon
    Name_5: breezy-eggplant-mastiff



```python

```


```python

```


```python

```


---
**Score: 5**
