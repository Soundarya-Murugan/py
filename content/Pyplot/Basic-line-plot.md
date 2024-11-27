---
title: Basic-Line-Plot
date: 2024-11-27
author: Your Name
cell_count: 11
score: 10
---

```python
#Basic Line Plot

```


```python
import matplotlib.pyplot as plt

```


```python
x = [1, 2, 3, 4, 5]
```


```python
y = [2, 3, 5, 7, 11]
```


```python
plt.plot(x, y, marker='o')
```




    [<matplotlib.lines.Line2D at 0x7f372d592fc0>]




    
![png](Basic-line-plot_files/Basic-line-plot_4_1.png)
    



```python
plt.title("Basic Line Plot")
```




    Text(0.5, 1.0, 'Basic Line Plot')




    
![png](Basic-line-plot_files/Basic-line-plot_5_1.png)
    



```python
plt.xlabel("X-axis")
```




    Text(0.5, 0, 'X-axis')




    
![png](Basic-line-plot_files/Basic-line-plot_6_1.png)
    



```python
plt.ylabel("Y-axis")
```




    Text(0, 0.5, 'Y-axis')




    
![png](Basic-line-plot_files/Basic-line-plot_7_1.png)
    



```python
plt.grid()
```


    
![png](Basic-line-plot_files/Basic-line-plot_8_0.png)
    



```python
plt.show()
```


```python

```


---
**Score: 10**
