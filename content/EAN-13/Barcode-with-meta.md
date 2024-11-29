---
title: Barcode-With-Meta
date: 2024-11-29
author: Your Name
cell_count: 11
score: 10
---

```python
import barcode



```


```python
from barcode.writer import ImageWriter

```


```python
from PIL import Image, ImageDraw, ImageFont


```


```python
# Create an EAN-13 barcode
ean = barcode.get_barcode_class('ean13')

```


```python
ean_code = ean('123456789012', writer=ImageWriter())


```


```python
# Generate the barcode image
barcode_image = ean_code.render()


```


```python
# Add custom text (metadata) to the image
draw = ImageDraw.Draw(barcode_image)

```


```python
font = ImageFont.load_default()


```


```python
# Add custom text to the barcode (e.g., Product Name)
product_name = "Product XYZ"

```


```python
draw.text((10, 10), product_name, font=font, fill='black')


```


```python
# Save the final barcode with the added metadata
barcode_image.save('ean13_with_metadata.png')
```


---
**Score: 10**
