# Quote_Scraping
# Goodreads Quote Scraper

## Description
This project is a **Python web scraping tool** that collects quotes and their authors from [Goodreads Quotes](https://www.goodreads.com/quotes).  
It uses **BeautifulSoup** and **requests** to extract the quotes from multiple pages and stores them in Python lists.  

This project is intended as a **learning exercise in web scraping, data extraction, and Python automation**. It can be extended to save quotes into a CSV or display them in a web app.

---

## Features
- Scrapes multiple pages of quotes from Goodreads.  
- Extracts both **quote text** and **author names**.  
- Stores the quotes and authors in Python lists.  
- Can be easily extended to save data in CSV or JSON.  

---

## Technologies Used
- Python 3.x  
- `requests` library (to fetch webpages)  
- `BeautifulSoup` from `bs4` (to parse HTML)  
- Optionally `pandas` for data storage  

---

## How to Use
1. Open the notebook `QUOTE_SCRAPING.ipynb` in Colab or locally.  
2. Run the scraper function to collect quotes from the desired number of pages.  
3. The scraped quotes and authors will be stored in the `quotes` and `authors` lists.  
4. You can combine them into a single list or save to a CSV if desired:

```python
import pandas as pd

df = pd.DataFrame({"Quote": quotes, "Author": authors})
df.to_csv("quotes.csv", index=False)
