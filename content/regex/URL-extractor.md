---
title: Url-Extractor
date: 2024-11-23
author: Your Name
cell_count: 9
score: 5
---

```python
#Finds and extracts all URLs from a given text.
```


```python
import re

```


```python
def extract_urls(text):
    url_regex = r'https?://(?:www\.)?\S+\.\S+'
    return re.findall(url_regex, text)


```


```python

# Test text

```


```python
text = """
Check out the following websites:
- https://www.example.com
- http://openai.com
- https://sub.domain.com/page
"""


```


```python
urls = extract_urls(text)

```


```python
print("Extracted URLs:")

```

    Extracted URLs:



```python
for url in urls:
    print(url)
```

    https://www.example.com
    http://openai.com
    https://sub.domain.com/page



```python

```


---
**Score: 5**
