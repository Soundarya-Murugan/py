---
title: Customize-Barcode-Specific
date: 2024-11-27
author: Your Name
cell_count: 7
score: 5
---

```python
import barcode


```


```python
from barcode.writer import ImageWriter


```


```python
ean = barcode.get_barcode_class('ean13')

```


```python
ean_code = ean('123456789012', writer=ImageWriter())


```


```python
# Customize the barcode
ean_code.writer.set_options({'text_distance': 2, 'font_size': 14, 'module_width': 0.2})

```


```python

# Save barcode with custom options
ean_code.save('custom_ean13')
```




    'custom_ean13.png'




```python

```


---
**Score: 5**
