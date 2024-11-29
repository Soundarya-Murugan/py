---
title: Matplot-Bars
date: 2024-11-29
author: Your Name
cell_count: 9
score: 5
---

```python
#Bar Color matplotlib bars
```


```python
#The bar() and barh() take the keyword argument color to set the color of the bars:
```


```python
import matplotlib.pyplot as plt
```


```python
import numpy as np
```


```python
x = np.array(["A", "B", "C", "D"])
```


```python
y = np.array([3, 8, 1, 10])
```


```python
plt.bar(x, y, color = "red")
```




    <BarContainer object of 4 artists>




    
![png](matplot-bars_files/matplot-bars_6_1.png)
    



```python
plt.show()
```


```python

```


---
**Score: 5**
