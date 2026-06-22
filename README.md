# WOB Product Sitemap Scraper

This project is a **Scrapy spider** that extracts product offer data from the WOB sitemap. It collects product information such as ISBN, SKU, price, availability, item condition, and currency, then saves the results into a CSV file.

## Project Overview

The spider starts from the WOB SEO sitemap, finds product sitemap links, visits each product page, reads structured JSON-LD product data, and extracts only products that are currently in stock.

## Data Extracted

The scraper collects the following fields:

* ISBN
* SKU
* Price
* Availability
* Item Condition
* Price Currency

## Output File

The scraped data is exported automatically to:

```text
wob_sitemap.csv
```

## Tools Used

* Python
* Scrapy
* Regex
* JSON

## How to Run

Install Scrapy:

```bash
pip install scrapy
```

Run the spider:

```bash
scrapy crawl wob_sitemap_spider
```

## Spider Name

```text
wob_sitemap_spider
```

