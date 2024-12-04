---
title: Horizontal Bar Chart
date: 2024-12-04
author: Your Name
cell_count: 11
score: 10
---

```python
# Horizontal Bar Chart
```


```python
import matplotlib.pyplot as plt
```


```python
# Data
```


```python
categories = ['A', 'B', 'C']
values = [23, 45, 30]
```


```python
# Plot
```


```python
plt.barh(categories, values, color='pink')
```




    <BarContainer object of 3 artists>




    
![png](horizontal_bar_chart_files/horizontal_bar_chart_5_1.png)
    



```python
plt.title("Horizontal Bar Chart")
```




    Text(0.5, 1.0, 'Horizontal Bar Chart')




    
![png](horizontal_bar_chart_files/horizontal_bar_chart_6_1.png)
    



```python
plt.xlabel("Values")
```




    Text(0.5, 0, 'Values')




    
![png](horizontal_bar_chart_files/horizontal_bar_chart_7_1.png)
    



```python
plt.ylabel("Categories")
```




    Text(0, 0.5, 'Categories')




    
![png](horizontal_bar_chart_files/horizontal_bar_chart_8_1.png)
    



```python
plt.show()
```


```python

```


---
**Score: 10**
