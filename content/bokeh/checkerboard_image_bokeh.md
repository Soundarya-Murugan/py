---
title: Checkerboard Image Bokeh
date: 2024-12-04
author: Your Name
cell_count: 10
score: 10
---

```python
#Generate a Checkerboard Image
```


```python
from PIL import Image
```


```python
# Generate a checkerboard pattern
```


```python
width, height = 400, 400
```


```python
img = Image.new('RGB', (width, height))
```


```python
pixels = img.load()
```


```python
# Create checkerboard pattern
```


```python
for y in range(height):
    for x in range(width):
        if (x // 50 + y // 50) % 2 == 0:
            pixels[x, y] = (0, 0, 0)  # Black
        else:
            pixels[x, y] = (255, 255, 255)  # White
```


```python
img.save('checkerboard_image.png')
```


```python

```


---
**Score: 10**
