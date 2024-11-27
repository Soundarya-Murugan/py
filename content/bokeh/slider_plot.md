---
title: Slider Plot
date: 2024-11-27
author: Your Name
cell_count: 9
score: 5
---

```python
#Slider PLot

```


```python
from bokeh.plotting import figure, output_file, save

```


```python
from bokeh.io import show

```


```python
from bokeh.models import Slider

```


```python
from bokeh.layouts import column

```


```python

output_file("slider_plot.html")

p = figure(title="Interactive Slider Plot", x_axis_label='X', y_axis_label='Y')

# Initial line
line = p.line([1, 2, 3, 4, 5], [6, 7, 2, 4, 5], line_width=2)


```


```python
def update(attr, old, new):
    line.data_source.data['y'] = [6*new, 7*new, 2*new, 4*new, 5*new]
    p.title.text = f"Interactive Slider Plot (Multiplier = {new})"

```


```python

slider = Slider(start=1, end=10, value=1, step=0.1, title="Multiplier")
slider.on_change('value', update)

show(column(p, slider))
```

    WARNING:bokeh.embed.util:
    You are generating standalone HTML/JS output, but trying to use real Python
    callbacks (i.e. with on_change or on_event). This combination cannot work.
    
    Only JavaScript callbacks may be used with standalone output. For more
    information on JavaScript callbacks with Bokeh, see:
    
        https://docs.bokeh.org/en/latest/docs/user_guide/interaction/js_callbacks.html
    
    Alternatively, to use real Python callbacks, a Bokeh server application may
    be used. For more information on building and running Bokeh applications, see:
    
        https://docs.bokeh.org/en/latest/docs/user_guide/server.html
    



```python

```


---
**Score: 5**
