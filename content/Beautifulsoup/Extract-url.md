---
title: Extract-Url
date: 2024-12-04
author: Your Name
cell_count: 14
score: 10
---

```python
#Image Source Scraping
```


```python
#Extract all image URLs (<img src="...">) from a webpage.
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
url = "https://books.toscrape.com/catalogue/category/books/poetry_23/index.html"
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
if response.status_code == 200:
    # Parse the HTML content with BeautifulSoup
    soup = BeautifulSoup(response.content, 'html.parser')
```


```python
    # Find all anchor tags
```


```python
    links = soup.find_all('a')
```


```python
    # Loop through all the links and print their href attributes
```


```python
    for link in links:
        href = link.get('href')
        print(href)
```


---
**Score: 10**
