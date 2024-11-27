---
title: Extract-Table-Soup
date: 2024-11-27
author: Your Name
cell_count: 17
score: 15
---

```python
#Extracting Table Data
```


```python
import requests
```


```python
from bs4 import BeautifulSoup
```


```python
# URL of the page to scrape
```


```python
url = "https://books.toscrape.com/catalogue/the-black-maria_991/index.html"
```


```python
# Fetch the HTML content using requests
```


```python
response = requests.get(url)
```


```python
# Check if the request was successful
```


```python
    # Parse the HTML content with BeautifulSoup
```


```python
    soup = BeautifulSoup(response.content, 'html.parser')
```


```python
    price_element = soup.select_one("#content_inner > article > table")
```


```python
 # Find the table (if present) and extract rows and columns
```


```python
if price_element:
    print("Price:", price_element.text)
else:
    print("Price not found")
```

    Price: 
    
    UPC1dfe412b8ac00530
    
    
    Product TypeBooks
    
    
    Price (excl. tax)£52.15
    
    
    Price (incl. tax)£52.15
    
    
    Tax£0.00
    
    
    Availability
    In stock (19 available)
    
    
    Number of reviews
    0
    
    



```python

```


```python

```


```python

```


```python

```


---
**Score: 15**
