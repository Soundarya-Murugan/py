---
title: Generate-Without-Text
date: 2024-11-29
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
# Disable text
ean_code.writer.set_options({'quiet_zone': 6, 'text': ''})

```


```python

# Save barcode without text
ean_code.save('ean13_no_text')
```




    'ean13_no_text.png'




```python

```


---
**Score: 5**
