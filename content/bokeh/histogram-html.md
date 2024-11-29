---
title: Histogram-Html
date: 2024-11-29
author: Your Name
cell_count: 12
score: 10
---

```python
#Histogram
```


```python
from bokeh.plotting import figure, output_file, save
```


```python
import numpy as np
```


```python
output_file("histogram_graph.html")
```


```python
# Generate random data
```


```python
data = np.random.normal(0, 0.5, 1000)

```


```python
# Create histogram
```


```python
p = figure(title="Histogram", tools="", x_axis_label='Value', y_axis_label='Frequency')

```


```python
hist, edges = np.histogram(data, bins=30)

```


```python
# Add histogram to plot
```


```python
p.quad(top=hist, bottom=0, left=edges[:-1], right=edges[1:], fill_color="skyblue", line_color="white")

save(p)

```




    '/home/soundarya/tact/pynotes/notebooks/bokeh/histogram_graph.html'




```python

```


---
**Score: 10**
