---
title: Extract-Hashtags
date: 2024-12-04
author: Your Name
cell_count: 6
score: 5
---

```python
#Extract Hashtags from Social Media Text
```


```python
import re
```


```python
import sys
```


```python
def extract_hashtags(text):
    hashtag_pattern = r'#\w+'
    hashtags = re.findall(hashtag_pattern, text)
    if hashtags:
        print("Hashtags found:")
        for hashtag in hashtags:
            print(hashtag)
    else:
        print("No hashtags found.")
```


```python
if __name__ == "__main__":
    if len(sys.argv) != 2:
        print("Usage: python script.py 'social media text'")
    else:
        input_text = sys.argv[1]
        extract_hashtags(input_text)
```

    Usage: python script.py 'social media text'



```python

```


---
**Score: 5**
