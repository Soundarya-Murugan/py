---
title: Handling-Nested-Dictionaries
date: 2024-11-27
author: Your Name
cell_count: 7
score: 5
---

```python
import magicattr

```


```python
class Person:
    def __init__(self, name, details):
        self.name = name
        self.details = details  # details is a dictionary with nested data



```


```python
# Create a Person instance
person = Person('Alice', {'address': {'city': 'Wonderland', 'zip': '12345'}})


```


```python
# Using magicattr to set the 'name' attribute
magicattr.set(person, 'name', 'Bob')


```


```python
# Directly manipulate the nested dictionary value
person.details['address']['city'] = 'Dreamland'

```


```python
# Using magicattr to get the 'name' attribute
name = magicattr.get(person, 'name')

```


```python
# Output the updated values
print(name)  # Expected Output: 'Bob'
print(person.details['address']['city'])  # Expected Output: 'Dreamland'
```


---
**Score: 5**
