---
title: Barcode-Generation
date: 2024-11-30
author: Your Name
cell_count: 6
score: 5
---

```python
import barcode


```


```python
from barcode.writer import ImageWriter

```


```python
# Create barcode
ean = barcode.get_barcode_class('ean13')

```


```python
ean_code = ean('123456789012', writer=ImageWriter())

```


```python

# Save as PNG file
ean_code.save('ean13_barcode')
```




    'ean13_barcode.png'




```python

```


---
**Score: 5**
