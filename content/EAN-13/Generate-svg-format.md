---
title: Generate-Svg-Format
date: 2024-11-27
author: Your Name
cell_count: 6
score: 5
---

```python
import barcode

```


```python
from barcode.writer import SVGWriter



```


```python
ean = barcode.get_barcode_class('ean13')

```


```python
ean_code = ean('123456789012', writer=SVGWriter())


```


```python
# Save as SVG
ean_code.save('ean13_barcode_svg')
```




    'ean13_barcode_svg.svg'




```python

```


---
**Score: 5**
