---
title: Extract-Img
date: 2024-11-30
author: Your Name
cell_count: 12
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
url = "https://books.toscrape.com/catalogue/category/books/poetry_23/index.html"
```


```python
response = requests.get(url)
```


```python
if response.status_code == 200:
    # Parse the HTML content with BeautifulSoup
    soup = BeautifulSoup(response.content, 'html.parser')
```


```python
    # Find all img tags
```


```python
    images = soup.find_all('img')
```


```python
    # Loop through all the images and print their 'src' attributes
```


```python
    for image in images:
        src = image.get('src')
        print(src)
```

    ../../../../media/cache/2c/da/2cdad67c44b002e7ead0cc35693c0e8b.jpg
    ../../../../media/cache/58/46/5846057e28022268153beff6d352b06c.jpg
    ../../../../media/cache/10/48/1048f63d3b5061cd2f424d20b3f9b666.jpg
    ../../../../media/cache/55/33/553310a7162dfbc2c6d19a84da0df9e1.jpg
    ../../../../media/cache/e9/20/e9203b733126c4a0832a1c7885dc27cf.jpg
    ../../../../media/cache/72/41/72417db983862010ef0c1a25de98c7d7.jpg
    ../../../../media/cache/f9/3b/f93b4a650f03a5d21f2436d7813f42c2.jpg
    ../../../../media/cache/38/64/386468a8c3e6b880664bf7885bf6f726.jpg
    ../../../../media/cache/25/54/2554431c797ec725eea50b3f8a83758c.jpg
    ../../../../media/cache/3f/41/3f4160ada0b16e3c64cd2d0dffe781c8.jpg
    ../../../../media/cache/c8/f2/c8f297fab080ddd02b3ed5c17b83af85.jpg
    ../../../../media/cache/93/d5/93d5c64abfad9ed6a0cb2e26f19f1a1e.jpg
    ../../../../media/cache/36/5b/365b3ab7ab72a6258873716aef6d5c1a.jpg
    ../../../../media/cache/b7/29/b7293f602efb0c17e305077f8175888a.jpg
    ../../../../media/cache/31/c7/31c7c5ce7b04d227aa36ecb250b9dad5.jpg
    ../../../../media/cache/7e/93/7e934132cd03486649fb492fe702f704.jpg
    ../../../../media/cache/9f/35/9f351ca1978128c60a3b7f85987075b3.jpg
    ../../../../media/cache/8f/46/8f46bb13feb3a4440a27dfcf688fbaa6.jpg
    ../../../../media/cache/df/ab/dfab1d94f9190df7c13b63a093a6d16e.jpg



```python

```


---
**Score: 10**
