---
title: Return-Img-Obj
date: 2024-11-29
author: Your Name
cell_count: 8
score: 5
---

```python
import barcode

```


```python
from barcode.writer import ImageWriter


```


```python
from PIL import Image


```


```python
ean = barcode.get_barcode_class('ean13')

```


```python
ean_code = ean('123456789012', writer=ImageWriter())


```


```python
# Return image object instead of saving
img = ean_code.render()


```


```python
# Show the image
img.show()
```


```python

```


---
**Score: 5**
