---
title: Adding-Annotations
date: 2024-11-27
author: Your Name
cell_count: 11
score: 10
---

```python
#Adding annotations
```


```python
import matplotlib.pyplot as plt
```


```python
x = [1, 2, 3, 4, 5]
```


```python
y = [1, 4, 9, 16, 25]
```


```python
plt.plot(x, y, marker="o")
for i, j in zip(x, y):
    plt.text(i, j+0.5, f"({i}, {j})")
```


    
![png](Adding-annotations_files/Adding-annotations_4_0.png)
    



```python

plt.title("Annotated Plot")

```




    Text(0.5, 1.0, 'Annotated Plot')




    
![png](Adding-annotations_files/Adding-annotations_5_1.png)
    



```python
plt.xlabel("X-axis")

```




    Text(0.5, 0, 'X-axis')




    
![png](Adding-annotations_files/Adding-annotations_6_1.png)
    



```python
plt.ylabel("Y-axis")

```




    Text(0, 0.5, 'Y-axis')




    
![png](Adding-annotations_files/Adding-annotations_7_1.png)
    



```python
plt.grid()

```


    
![png](Adding-annotations_files/Adding-annotations_8_0.png)
    



```python
plt.show()
```


```python

```


---
**Score: 10**
