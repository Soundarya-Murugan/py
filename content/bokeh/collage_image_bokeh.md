---
title: Collage Image Bokeh
date: 2024-12-04
author: Your Name
cell_count: 11
score: 10
---

```python
#Create a Collage of Images
```


```python
from PIL import Image
```


```python
# Create a collage with multiple images
```


```python
img1 = Image.new('RGB', (100, 100), color=(255, 0, 0))
```


```python
img2 = Image.new('RGB', (100, 100), color=(0, 255, 0))
```


```python
img3 = Image.new('RGB', (100, 100), color=(0, 0, 255))
```


```python
collage = Image.new('RGB', (300, 100))
```


```python
collage.paste(img1, (0, 0))
```


```python
collage.paste(img2, (100, 0))
collage.paste(img3, (200, 0))
```


```python
collage.save('collage_image.png')
```


```python

```


---
**Score: 10**
