---
title: Multipleplots-Pyplot
date: 2024-12-04
author: Your Name
cell_count: 27
score: 25
---

```python
#Using pyplot library get multiple chart
```


```python
#create a sequence of plots with varying styles, datasets, or configurations
```


```python
import matplotlib.pyplot as plt
```


```python
import numpy as np
```


```python
# Data for plotting
```


```python
x = np.linspace(0, 10, 100)
```


```python
y1 = np.sin(x)
```


```python
y2 = np.cos(x)
```


```python
y3 = np.tan(x)
```


```python
# First plot - Sinusoidal curve
```


```python
plt.figure(1)
plt.plot(x, y1, label='sin(x)', color='blue')
plt.title('Sine Wave')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.grid(True)
plt.legend(loc='upper right')
plt.savefig('plot1_sine_wave.png')
plt.close()
```


```python
# Second plot - Cosine curve
```


```python
plt.figure(2)
plt.plot(x, y2, label='cos(x)', color='green')
plt.title('Cosine Wave')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.grid(True)
plt.legend(loc='upper right')
plt.savefig('plot2_cosine_wave.png')
plt.close()
```


```python
# Third plot - Tangent curve with limits
```


```python
plt.figure(3)
plt.plot(x, y3, label='tan(x)', color='red')
plt.ylim(-10, 10)  # limit y-axis to avoid infinite values at pi/2
plt.title('Tangent Wave')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.grid(True)
plt.legend(loc='upper right')
plt.savefig('plot3_tangent_wave.png')
plt.close()
```


```python
# Fourth plot - Subplots of sine and cosine
```


```python
fig, axs = plt.subplots(2)
axs[0].plot(x, y1, label='sin(x)', color='blue')
axs[0].set_title('Sine Wave')
axs[0].set_xlabel('X-axis')
axs[0].set_ylabel('Y-axis')
axs[0].grid(True)
axs[0].legend(loc='upper right')

axs[1].plot(x, y2, label='cos(x)', color='green')
axs[1].set_title('Cosine Wave')
axs[1].set_xlabel('X-axis')
axs[1].set_ylabel('Y-axis')
axs[1].grid(True)
axs[1].legend(loc='upper right')

plt.tight_layout()
plt.savefig('plot4_subplots_sine_cosine.png')
plt.close()

```


```python
# Fifth plot - Scatter plot
```


```python
plt.figure(5)
y5 = np.random.rand(100)
plt.scatter(x, y5, color='purple', label='Random Data')
plt.title('Scatter Plot')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.grid(True)
plt.legend(loc='upper right')
plt.savefig('plot5_scatter_plot.png')
plt.close()
```


```python
# Sixth plot - Histogram
```


```python
plt.figure(6)
data = np.random.randn(1000)
plt.hist(data, bins=30, color='orange', edgecolor='black')
plt.title('Histogram')
plt.xlabel('Value')
plt.ylabel('Frequency')
plt.grid(True)
plt.savefig('plot6_histogram.png')
plt.close()
```


```python
# Seventh plot - Pie chart
```


```python
plt.figure(7)
labels = ['A', 'B', 'C', 'D']
sizes = [15, 30, 45, 10]
plt.pie(sizes, labels=labels, autopct='%1.1f%%', colors=['red', 'blue', 'green', 'yellow'])
plt.title('Pie Chart')
plt.savefig('plot7_pie_chart.png')
plt.close()
```


```python
# Eighth plot - Bar chart
```


```python
plt.figure(8)
categories = ['Category 1', 'Category 2', 'Category 3']
values = [20, 35, 30]
plt.bar(categories, values, color=['purple', 'blue', 'green'])
plt.title('Bar Chart')
plt.xlabel('Categories')
plt.ylabel('Values')
plt.grid(True)
plt.savefig('plot8_bar_chart.png')
plt.close()
```


```python
print("Plots have been saved successfully!")
```

    Plots have been saved successfully!



```python

```


---
**Score: 25**
