---
title: Extract-All-Link
date: 2024-11-27
author: Your Name
cell_count: 20
score: 20
---

```python
#Using CSS Selectors to Find Elements
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
if response.status_code == 200:
    html_content = response.content
    soup = BeautifulSoup(html_content, 'html.parser')

```


```python
    # Extract the book title
```


```python
title = soup.select_one('.product_main h1').get_text()

    # Extract the price
```


```python
    price = soup.select_one('.price_color').get_text()
```


```python

    # Extract the availability
```


```python
    availability = soup.select_one('.availability').get_text(strip=True)
```


```python
# Extract the product description
```


```python
    description = soup.select_one('#product_description + p')
    description_text = description.get_text() if description else "No description available."
```


```python
    # Extract product information from the table
```


```python
    product_info = {}
    table = soup.select('table.table.table-striped tr')
    for row in table:
        th = row.find('th').get_text().strip()
        td = row.find('td').get_text().strip()
        product_info[th] = td
```


```python
    # Print extracted information
    print(f"Title: {title}")
    print(f"Price: {price}")
    print(f"Availability: {availability}")
    print(f"Description: {description_text}")
    print("Product Information:")
    for key, value in product_info.items():
        print(f"  {key}: {value}")

```

    Title: The Black Maria
    Price: £52.15
    Availability: In stock (19 available)
    Description: Praise for Aracelis Girmay:"[Girmay's] every loss—she calls them estrangements—is a yearning for connection across time and place; her every fragment is a bulwark against ruin." — O, The Oprah Magazine "In Aracelis Girmay we have a poet who collects, polishes, and shares stories with such brilliant invention, tenderness, and intellectual liveliness that it is understandabl Praise for Aracelis Girmay:"[Girmay's] every loss—she calls them estrangements—is a yearning for connection across time and place; her every fragment is a bulwark against ruin." — O, The Oprah Magazine "In Aracelis Girmay we have a poet who collects, polishes, and shares stories with such brilliant invention, tenderness, and intellectual liveliness that it is understandable that we think of her as the blessed curator of our collective histories. There is in her art the vulnerability of one who lives inside of the stories that she gathers in this remarkable collection. Her poems set off alarms even as they transform the world she inhabits, showing us, in the process, exactly what she asks of Romare Bearden’s art: ‘…how not to // assign all blackness near the sea / a captivity.’ This is one of the many sweet contradictions in the black maria, which ‘is a black flag / wounding the pastoral.’ I am deeply thankful that we have a poet of her unique and singular talent writing today." —Kwame DawesTaking its name from the moon's dark plains, misidentified as seas by early astronomers, the black maria investigates African diasporic histories, the consequences of racism within American culture, and the question of human identity. Central to this project is a desire to recognize the lives of Eritrean refugees who have been made invisible by years of immigration crisis, refugee status, exile, and resulting statelessness. The recipient of a 2015 Whiting Award for Poetry, Girmay's newest collection elegizes and celebrates life, while wrestling with the humanistic notion of seeing beyond: seeing violence, seeing grace, and seeing each other better."to the sea"great storage house, historyon which we rode, we touchedthe brief pulse of your flutteringpages, spelled with salt & life,your rage, your indifferenceyour gentleness washing our feet,all of you going onwhether or not we live,to you we bring our carnationsyellow & pink, how they floatlike bright sentences atopyour memory's dark hairAracelis Girmay is the author of three poetry collections, the black maria; Kingdom Animalia, which won the Isabella Gardner Award and was a finalist for the NBCC Award; and Teeth. The recipient of a 2015 Whiting Award, she has received grants and fellowships from the Jerome, Cave Canem, and Watson foundations, as well as Civitella Ranieri and the NEA. She currently teaches at Hampshire College's School for Interdisciplinary Arts and in Drew University's low residency MFA program. Originally from Santa Ana, California, she splits her time between New York and Amherst, Massachusetts. ...more
    Product Information:
      UPC: 1dfe412b8ac00530
      Product Type: Books
      Price (excl. tax): £52.15
      Price (incl. tax): £52.15
      Tax: £0.00
      Availability: In stock (19 available)
      Number of reviews: 0



```python

```


---
**Score: 20**
