ebScraper JSON Sitemap Tester

A Python/Google Colab tool for testing and validating WebScraper.io JSON sitemaps, extracting data through CSS selectors, handling the :contains() pseudo-class, and exporting results into a clean CSV file.

This tool is designed to help web scrapers quickly verify whether their sitemap selectors still work on target pages — especially when websites change structure or introduce dynamic content.

🚀 Overview

This project contains:

A Google Colab notebook (webscraper_test1.ipynb) for interactively testing JSON sitemaps

Real sitemap files extracted from several financial product websites

A fully working Python workflow using BeautifulSoup, Requests, Pandas, and RegEx

Output generation into a CSV file (json_test_results.csv)

The purpose is to validate scraper configurations before running full crawls or automated scrapers.

📌 Included Files
webscraper_test1.ipynb      # main Google Colab notebook
21shares_ALL.json           # real sitemap used for testing 21Shares product pages
3iQ_ALL.json                # real sitemap used for testing 3iQ fund pages


These JSON files contain real CSS selectors, including:

product names

tickers

ISIN values

NAV / AUM fields

management fees

table-based selectors

nested elements

text extraction with regex

They are perfect examples of real-world scraping challenges.

-- What the Notebook Does

- Uploads any WebScraper.io JSON sitemap
- Loads all selectors automatically
- Supports :contains("text") pseudo-class
- Scrapes target URLs with BeautifulSoup
- Extracts and cleans text fields
- Applies optional regex filters
- Returns "(not found)" when selectors fail
- Outputs results into json_test_results.csv

This makes it extremely useful for:

debugging scrapers

updating broken selectors

validating website changes

testing multiple pages at once

--How to Use (Google Colab)

Open the notebook in Google Colab

Run all cells

Upload your WebScraper sitemap (.json)

Wait for the extractor to process each URL

Download your CSV file with the results

Ideal for both beginners and advanced users.

--Technologies Used

Python

Google Colab

BeautifulSoup

Requests

Pandas

RegEx

JSON Parsing

CSS Selectors
