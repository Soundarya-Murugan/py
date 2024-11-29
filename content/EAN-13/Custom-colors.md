---
title: Custom-Colors
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

# Create an EAN-13 barcode
ean = barcode.get_barcode_class('ean13')

```


```python
ean_code = ean('123456789012', writer=ImageWriter())


```


```python
# Set custom colors for barcode
options = {
    'background': 'white',  # Background color
    'foreground': 'black',  # Barcode color
}


```


```python
# Apply the color options and save the barcode
ean_code.writer.set_options(options)

```


```python
ean_code.save('ean13_custom_colors')
```




    'ean13_custom_colors.png'




```python

```


---
**Score: 5**
