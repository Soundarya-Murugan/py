---
title: Extract-Para
date: 2024-12-04
author: Your Name
cell_count: 15
score: 15
---

```python
#. Paragraph and Heading Scraping
```


```python
#Scrape all <p> tags and <h1> to <h6> headings from a webpage.
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
    # Find all p tags (paragraphs)
```


```python
    paragraphs = soup.find_all(['p','h1','h2','h3','h4','h5','h6'])
```


```python
    # Loop through all the paragraphs and print their text
```


```python
    for para in paragraphs:
        print(para.get_text())
```

    Poetry
    
    
    
    
    
    
    
    A Light in the ...
    £51.77
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    The Black Maria
    £52.15
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Shakespeare's Sonnets
    £20.66
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Olio
    £23.88
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    You can't bury them ...
    £33.63
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Slow States of Collapse: ...
    £57.31
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Untitled Collection: Sabbath Poems ...
    £14.27
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Poems That Make Grown ...
    £14.19
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Night Sky with Exit ...
    £41.05
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    salt.
    £46.78
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Quarter Life Poetry: Poems ...
    £50.89
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Out of Print: City ...
    £53.64
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Les Fleurs du Mal
    £29.04
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Howl and Other Poems
    £40.45
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Leave This Song Behind: ...
    £51.17
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    The Collected Poems of ...
    £15.42
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    The Crossover
    £38.77
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Booked
    £17.49
    
    
        
            In stock
        
    
    
    
    
    
    
    
    
    Twenty Love Poems and ...
    £30.95
    
    
        
            In stock
        
    



```python

```


---
**Score: 15**
