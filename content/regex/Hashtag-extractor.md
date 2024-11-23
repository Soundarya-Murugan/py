---
title: Hashtag-Extractor
date: 2024-11-23
author: Your Name
cell_count: 7
score: 5
---

```python
import re


```


```python
def extract_hashtags(text):
    hashtag_regex = r'#\w+'
    return re.findall(hashtag_regex, text)
```


```python
# Test text
text = """
Today is a great day! #sunny #weekend #fun
Let's enjoy the #sunshine and have a #picnic.
"""



```


```python
hashtags = extract_hashtags(text)

```


```python
print("Extracted hashtags:")

```

    Extracted hashtags:



```python
for hashtag in hashtags:
    print(hashtag)
```

    #sunny
    #weekend
    #fun
    #sunshine
    #picnic



```python

```


---
**Score: 5**
