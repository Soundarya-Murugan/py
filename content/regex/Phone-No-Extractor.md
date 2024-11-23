---
title: Phone-No-Extractor
date: 2024-11-23
author: Your Name
cell_count: 10
score: 10
---

```python
#Extracts phone numbers in various formats from a block of text.
```


```python
import re
```


```python
def extract_phone_numbers(text):
    phone_regex = r'\+?\d[\d\s()-]{7,}\d'
    return re.findall(phone_regex, text)

```


```python
#Test Text
```


```python
# Test text
text = """
Here are some phone numbers:
- +1-800-555-1234
- (123) 456 7890
- 1234567890
- +91 9876543210
"""

```


```python
#Phone Numbers 
```


```python
phones = extract_phone_numbers(text)
```


```python
print("Extracted phone numbers:")
```

    Extracted phone numbers:



```python
for phone in phones:
    print(phone)
```

    +1-800-555-1234
    - (123) 456 7890
    - 1234567890
    +91 9876543210



```python

```


---
**Score: 10**
