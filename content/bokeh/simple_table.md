---
title: Simple Table
date: 2024-11-23
author: Your Name
cell_count: 10
score: 10
---

```python
#Simple Tab

```


```python
from bokeh.models import ColumnDataSource, DataTable, TableColumn
```


```python
from bokeh.plotting import output_file, save

```


```python
output_file("simple_table.html")

```


```python

data = {
    'name': ['Alice', 'Bob', 'Charlie'],
    'age': [24, 30, 22],
    'city': ['New York', 'Los Angeles', 'Chicago']
}


```


```python
source = ColumnDataSource(data)


```


```python
columns = [
    TableColumn(field="name", title="Name"),
    TableColumn(field="age", title="Age"),
    TableColumn(field="city", title="City")
]

```


```python
#Table Column Data
```


```python

data_table = DataTable(source=source, columns=columns, width=400, height=280)

save(data_table)

```




    '/home/soundarya/tact/pynotes/notebooks/bokeh/simple_table.html'




```python

```


---
**Score: 10**
