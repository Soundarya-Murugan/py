---
title: Embed-Gui
date: 2024-11-29
author: Your Name
cell_count: 13
score: 10
---

```python
import tkinter as tk

```


```python
from tkinter import PhotoImage

```


```python
import barcode

```


```python
from barcode.writer import ImageWriter

```


```python
from PIL import ImageTk


```


```python
# Generate barcode
ean = barcode.get_barcode_class('ean13')

```


```python
ean_code = ean('123456789012', writer=ImageWriter())

```


```python
barcode_img = ean_code.render()


```


```python
# Tkinter window setup
root = tk.Tk()

```


```python
root.title("EAN-13 Barcode")
# Convert barcode to ImageTk format
photo = ImageTk.PhotoImage(barcode_img)


```


```python
# Label to display the barcode
label = tk.Label(root, image=photo)
label.pack()


```


```python
# Run the Tkinter event loop
root.mainloop()
```


```python

```


---
**Score: 10**
