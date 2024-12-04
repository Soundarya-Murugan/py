---
title: Matplot-Grid
date: 2024-12-04
author: Your Name
cell_count: 14
score: 10
---

```python
#Add Grid Lines to a Plot
```


```python
import numpy as np
```


```python
import matplotlib.pyplot as plt

```


```python
x = np.array([80, 85, 90, 95, 100, 105, 110, 115, 120, 125])
```


```python
y = np.array([240, 250, 260, 270, 280, 290, 300, 310, 320, 330])
```


```python
plt.title("Sports Watch Data")
```




    Text(0.5, 1.0, 'Sports Watch Data')




    
![png](matplot-grid_files/matplot-grid_5_1.png)
    



```python

```


```python
plt.xlabel("Average Pulse")
```




    Text(0.5, 0, 'Average Pulse')




    
![png](matplot-grid_files/matplot-grid_7_1.png)
    



```python
plt.ylabel("Calorie Burnage")
```




    Text(0, 0.5, 'Calorie Burnage')




    
![png](matplot-grid_files/matplot-grid_8_1.png)
    



```python
plt.plot(x, y)
```




    [<matplotlib.lines.Line2D at 0x7f5d2cf4be00>]




    
![png](matplot-grid_files/matplot-grid_9_1.png)
    



```python
#With Pyplot, you can use the grid() function to add grid lines to the plot.
```


```python
plt.grid()
```


    
![png](matplot-grid_files/matplot-grid_11_0.png)
    



```python
plt.show()
```


```python

```


---
**Score: 10**
