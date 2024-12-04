---
title: Matplotlib-Histogram
date: 2024-12-04
author: Your Name
cell_count: 21
score: 20
---

```python
#Histogram with Normal Distribution Fit
```


```python
import matplotlib.pyplot as plt
```


```python
import numpy as np
```


```python
from scipy.stats import norm
```


```python
# Data
```


```python
data = np.random.normal(0, 1, 1000)
```


```python
# Plotting
```


```python
plt.figure(figsize=(10, 6))
```


```python
plt.hist(data, bins=30, density=True, alpha=0.6, color='g')
```


```python
# Fit normal distribution
```


```python
mu, std = norm.fit(data)
```


```python
xmin, xmax = plt.xlim()
```


```python
x = np.linspace(xmin, xmax, 100)
```


```python
p = norm.pdf(x, mu, std)
```


```python
plt.plot(x, p, 'k', linewidth=2)
```


```python
# Customizing
```


```python
plt.title(f"Histogram with Normal Distribution Fit\nμ={mu:.2f}, σ={std:.2f}")
plt.xlabel("Value")
plt.ylabel("Frequency")
plt.show()
```


```python

```


```python

```


```python

```


```python

```


---
**Score: 20**
