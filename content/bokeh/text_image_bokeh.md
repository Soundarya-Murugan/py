---
title: Text Image Bokeh
date: 2024-12-04
author: Your Name
cell_count: 9
score: 5
---

```python
#Generate an Image with Text
```


```python
from PIL import Image, ImageDraw, ImageFont
```


```python
# Create a blank image with white background
```


```python
img = Image.new('RGB', (400, 100), color=(255, 255, 255))
```


```python
draw = ImageDraw.Draw(img)
```


```python
# Load font and add text
```


```python
font = ImageFont.load_default()
draw.text((50, 40), "Hello, Pillow!", font=font, fill=(0, 0, 0))
```


```python
img.save('text_image.png')
```


```python

```


---
**Score: 5**
