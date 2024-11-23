---
title: Pie-Chart-Graph
date: 2024-11-23
author: Your Name
cell_count: 21
score: 20
---

```python
#Pie chart
```


```python
from math import pi
```


```python
from bokeh.io import output_file, save

```


```python
from bokeh.palettes import Category20c
```


```python
from bokeh.plotting import figure

```


```python
from bokeh.transform import cumsum
```


```python
import pandas as pd

```


```python
# Output to an HTML file
```


```python
output_file("pie_chart_graph.html")

```


```python
# Create the data

```


```python
data = pd.DataFrame({
    'fruits': ['Apple', 'Banana', 'Cherry', 'Grape', 'Orange'],
    'value': [50, 30, 15, 10, 20]
})


```


```python
# Calculate the angle for each slice of the pie

```


```python
data['angle'] = data['value'] / data['value'].sum() * 2 * pi

```


```python
# Use Category20c[5] to get exactly five colors

```


```python
data['color'] = Category20c[5]


```


```python
# Create a figure

```


```python
p = figure(title="Pie Chart", toolbar_location=None, tools="hover", 
           tooltips="@fruits: @value", x_range=(-0.5, 1.0))

```


```python
# Add wedges for each fruit
```


```python
p.wedge(x=0, y=1, radius=0.4, 
        start_angle=cumsum('angle', include_zero=True), end_angle=cumsum('angle'),
        line_color="white", fill_color='color', legend_field='fruits', source=data)

```




<div style="display: table;"><div style="display: table-row;"><div style="display: table-cell;"><b title="bokeh.models.renderers.glyph_renderer.GlyphRenderer">GlyphRenderer</b>(</div><div style="display: table-cell;">id&nbsp;=&nbsp;'p1079', <span id="p1085" style="cursor: pointer;">&hellip;)</span></div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">context_menu&nbsp;=&nbsp;None,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">coordinates&nbsp;=&nbsp;None,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">data_source&nbsp;=&nbsp;ColumnDataSource(id='p1070', ...),</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">glyph&nbsp;=&nbsp;Wedge(id='p1076', ...),</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">group&nbsp;=&nbsp;None,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">hover_glyph&nbsp;=&nbsp;None,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">js_event_callbacks&nbsp;=&nbsp;{},</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">js_property_callbacks&nbsp;=&nbsp;{},</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">level&nbsp;=&nbsp;'glyph',</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">muted&nbsp;=&nbsp;False,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">muted_glyph&nbsp;=&nbsp;Wedge(id='p1078', ...),</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">name&nbsp;=&nbsp;None,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">nonselection_glyph&nbsp;=&nbsp;Wedge(id='p1077', ...),</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">propagate_hover&nbsp;=&nbsp;False,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">selection_glyph&nbsp;=&nbsp;'auto',</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">subscribed_events&nbsp;=&nbsp;PropertyValueSet(),</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">syncable&nbsp;=&nbsp;True,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">tags&nbsp;=&nbsp;[],</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">view&nbsp;=&nbsp;CDSView(id='p1080', ...),</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">visible&nbsp;=&nbsp;True,</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">x_range_name&nbsp;=&nbsp;'default',</div></div><div class="p1084" style="display: none;"><div style="display: table-cell;"></div><div style="display: table-cell;">y_range_name&nbsp;=&nbsp;'default')</div></div></div>
<script>
(function() {
  let expanded = false;
  const ellipsis = document.getElementById("p1085");
  ellipsis.addEventListener("click", function() {
    const rows = document.getElementsByClassName("p1084");
    for (let i = 0; i < rows.length; i++) {
      const el = rows[i];
      el.style.display = expanded ? "none" : "table-row";
    }
    ellipsis.innerHTML = expanded ? "&hellip;)" : "&lsaquo;&lsaquo;&lsaquo;";
    expanded = !expanded;
  });
})();
</script>





```python
# Hide the axis and grid
p.axis.axis_label = None
p.axis.visible = False
p.grid.grid_line_color = None

# Save the plot
save(p)
```




    '/home/soundarya/tact/pynotes/notebooks/bokeh/pie_chart_graph.html'




```python

```


---
**Score: 20**
