---
title: Table-Example
date: 2024-11-29
author: Your Name
cell_count: 10
score: 10
---

```python
#Creating table in plot
```


```python
import matplotlib.pyplot as plt

```


```python
data = [
    ["Alice", 24, "Engineer"],
    ["Bob", 27, "Data Scientist"],
    ["Charlie", 22, "Teacher"]
]
```


```python
columns = ("Name", "Age", "Occupation")
```


```python
fig, ax = plt.subplots()
```


    
![png](Table-example_files/Table-example_4_0.png)
    



```python
ax.axis("tight")
```




    (-0.05500000000000001,
     0.05500000000000001,
     -0.05500000000000001,
     0.05500000000000001)




```python
ax.axis("off")

```




    (-0.05500000000000001,
     0.05500000000000001,
     -0.05500000000000001,
     0.05500000000000001)




```python
table = ax.table(cellText=data, colLabels=columns, cellLoc="center", loc="center")

```


```python
plt.title("Simple Table Example")

```




    Text(0.5, 1.0, 'Simple Table Example')




    
![png](Table-example_files/Table-example_8_1.png)
    



```python
plt.show()
```


---
**Score: 10**
