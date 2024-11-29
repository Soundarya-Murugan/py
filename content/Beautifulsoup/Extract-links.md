---
title: Extract-Links
date: 2024-11-30
author: Your Name
cell_count: 14
score: 10
---

```python
# Link Extraction
```


```python
# Extract all the hyperlinks (<a href="...">) from a webpage.
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

    ../../../../index.html
    ../../../../index.html
    ../../books_1/index.html
    ../../books_1/index.html
    ../travel_2/index.html
    ../mystery_3/index.html
    ../historical-fiction_4/index.html
    ../sequential-art_5/index.html
    ../classics_6/index.html
    ../philosophy_7/index.html
    ../romance_8/index.html
    ../womens-fiction_9/index.html
    ../fiction_10/index.html
    ../childrens_11/index.html
    ../religion_12/index.html
    ../nonfiction_13/index.html
    ../music_14/index.html
    ../default_15/index.html
    ../science-fiction_16/index.html
    ../sports-and-games_17/index.html
    ../add-a-comment_18/index.html
    ../fantasy_19/index.html
    ../new-adult_20/index.html
    ../young-adult_21/index.html
    ../science_22/index.html
    index.html
    ../paranormal_24/index.html
    ../art_25/index.html
    ../psychology_26/index.html
    ../autobiography_27/index.html
    ../parenting_28/index.html
    ../adult-fiction_29/index.html
    ../humor_30/index.html
    ../horror_31/index.html
    ../history_32/index.html
    ../food-and-drink_33/index.html
    ../christian-fiction_34/index.html
    ../business_35/index.html
    ../biography_36/index.html
    ../thriller_37/index.html
    ../contemporary_38/index.html
    ../spirituality_39/index.html
    ../academic_40/index.html
    ../self-help_41/index.html
    ../historical_42/index.html
    ../christian_43/index.html
    ../suspense_44/index.html
    ../short-stories_45/index.html
    ../novels_46/index.html
    ../health_47/index.html
    ../politics_48/index.html
    ../cultural_49/index.html
    ../erotica_50/index.html
    ../crime_51/index.html
    ../../../a-light-in-the-attic_1000/index.html
    ../../../a-light-in-the-attic_1000/index.html
    ../../../the-black-maria_991/index.html
    ../../../the-black-maria_991/index.html
    ../../../shakespeares-sonnets_989/index.html
    ../../../shakespeares-sonnets_989/index.html
    ../../../olio_984/index.html
    ../../../olio_984/index.html
    ../../../you-cant-bury-them-all-poems_961/index.html
    ../../../you-cant-bury-them-all-poems_961/index.html
    ../../../slow-states-of-collapse-poems_960/index.html
    ../../../slow-states-of-collapse-poems_960/index.html
    ../../../untitled-collection-sabbath-poems-2014_953/index.html
    ../../../untitled-collection-sabbath-poems-2014_953/index.html
    ../../../poems-that-make-grown-women-cry_824/index.html
    ../../../poems-that-make-grown-women-cry_824/index.html
    ../../../night-sky-with-exit-wounds_822/index.html
    ../../../night-sky-with-exit-wounds_822/index.html
    ../../../salt_731/index.html
    ../../../salt_731/index.html
    ../../../quarter-life-poetry-poems-for-the-young-broke-and-hangry_727/index.html
    ../../../quarter-life-poetry-poems-for-the-young-broke-and-hangry_727/index.html
    ../../../out-of-print-city-lights-spotlight-no-14_536/index.html
    ../../../out-of-print-city-lights-spotlight-no-14_536/index.html
    ../../../les-fleurs-du-mal_530/index.html
    ../../../les-fleurs-du-mal_530/index.html
    ../../../howl-and-other-poems_522/index.html
    ../../../howl-and-other-poems_522/index.html
    ../../../leave-this-song-behind-teen-poetry-at-its-best_474/index.html
    ../../../leave-this-song-behind-teen-poetry-at-its-best_474/index.html
    ../../../the-collected-poems-of-wb-yeats-the-collected-works-of-wb-yeats-1_441/index.html
    ../../../the-collected-poems-of-wb-yeats-the-collected-works-of-wb-yeats-1_441/index.html
    ../../../the-crossover_398/index.html
    ../../../the-crossover_398/index.html
    ../../../booked_365/index.html
    ../../../booked_365/index.html
    ../../../twenty-love-poems-and-a-song-of-despair_91/index.html
    ../../../twenty-love-poems-and-a-song-of-despair_91/index.html



```python

```


---
**Score: 10**
