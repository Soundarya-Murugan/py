---
title: Matplotlib Table
date: 2024-11-30
author: Your Name
cell_count: 8
score: 5
---

```python
#Table with Matplotlib
```


```python
import matplotlib.pyplot as plt
```


```python
# Data for table
```


```python
data = [['Alice', 85, 'A'],
        ['Bob', 78, 'B'],
        ['Charlie', 92, 'A+']]
```


```python
column_labels = ('Name', 'Score', 'Grade')
```


```python
# Plot
```


```python
fig, ax = plt.subplots()
ax.axis('tight')
ax.axis('off')
ax.table(cellText=data, colLabels=column_labels, loc='center')

plt.title("Table Example")
plt.show()
```


    
![png](matplotlib_table_files/matplotlib_table_6_0.png)
    



```python

```


---
**Score: 5**
