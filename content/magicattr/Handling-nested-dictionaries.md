---
title: Handling-Nested-Dictionaries
date: 2024-11-22
author: Your Name
cell_count: 2
score: 0
---

```python
import magicattr

class Person:
    def __init__(self, name, details):
        self.name = name
        self.details = details  # details is a dictionary with nested data

# Create a Person instance
person = Person('Alice', {'address': {'city': 'Wonderland', 'zip': '12345'}})

# Using magicattr to set the 'name' attribute
magicattr.set(person, 'name', 'Bob')

# Directly manipulate the nested dictionary value
person.details['address']['city'] = 'Dreamland'

# Using magicattr to get the 'name' attribute
name = magicattr.get(person, 'name')

# Output the updated values
print(name)  # Expected Output: 'Bob'
print(person.details['address']['city'])  # Expected Output: 'Dreamland'

```

    Bob
    Dreamland



```python

```


---
**Score: 0**
