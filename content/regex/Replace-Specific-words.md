---
title: Replace-Specific-Words
date: 2024-11-22
author: Your Name
cell_count: 7
score: 5
---

```python
import re

```


```python

def replace_words(text, word_dict):
    for word, replacement in word_dict.items():
        pattern = r'\b' + re.escape(word) + r'\b'
        text = re.sub(pattern, replacement, text)
    return text



```


```python
text = "I love Python. Python is awesome."

```


```python
word_dict = {"Python": "Java"}

```


```python
modified_text = replace_words(text, word_dict)

```


```python
print("Modified text:", modified_text)
```

    Modified text: I love Java. Java is awesome.



```python

```


---
**Score: 5**
