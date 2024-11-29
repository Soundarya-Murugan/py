---
title: Histogram
date: 2024-11-30
author: Your Name
cell_count: 5
score: 5
---

```python
#Histogram
```


```python
import matplotlib.pyplot as plt
```


```python
import numpy as np
```


```python
data = np.random.randn(1000)
plt.hist(data, bins=30, color="purple", alpha=0.7)
plt.title("Histogram")
plt.xlabel("Data values")
plt.ylabel("Frequency")
plt.show()
```


    
![png](Histogram_files/Histogram_3_0.png)
    



```python

```


---
**Score: 5**
