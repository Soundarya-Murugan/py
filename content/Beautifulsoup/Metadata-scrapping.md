---
title: Metadata-Scrapping
date: 2024-11-30
author: Your Name
cell_count: 11
score: 10
---

```python
#Webpage Metadata Scraping
```


```python
#Extract metadata such as <meta name="description"> and <meta name="keywords">.
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
    soup = BeautifulSoup(response.content, 'html.parser')

    description = soup.find('meta', {'name': 'description'})
    description_data = description['content'] if description else "No description found"

    keywords = soup.find('meta', {'name': 'keywords'})
    keywords_data = keywords['content'] if keywords else "No keyword found"
    
    print("Description of the book:", description_data)
    print("Keywords of the book:", keywords_data)


else:
    print("Failed to get the page.", response.status_code)
```

    Description of the book: 
        
    
    Keywords of the book: No keyword found



```python

```


---
**Score: 10**
