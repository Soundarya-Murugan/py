---
title: Reversed
date: 2024-11-29
author: Your Name
cell_count: 3
score: 0
---

```python
def reverse_words(sentence):
    """
    Given a sentence, reverse the order of words in it.

    Args:
    sentence: A string representing the input sentence.

    Returns:
    A string with words in reversed order.
    """

    # Split the sentence into words
    words = sentence.split()

    reversed_sentence = ' '.join(reversed(words))

    

    # do your code

    return reversed_sentence

# Test cases
# print(reverse_words("Hello World"))  # Output: "World Hello"
# print(reverse_words("Python is awesome"))  # Output: "awesome is Python"
# print(reverse_words("Coding test in Python"))  # Output: "Python in test Coding"

```


```python
print(reverse_words("Python is awesome"))
```

    awesome is Python



```python

```


---
**Score: 0**
