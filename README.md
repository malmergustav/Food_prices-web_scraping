# Project Name: Mathem-Hemkop-Scraper

## Description

This project provides a web scraping tool using Selenium and BeautifulSoup to extract information on discounted products from the Mathem and Hemkop websites. It retrieves data on product names, original prices, and sales prices, allowing users to analyze savings and price distributions. Furthermore, it provides visualizations illustrating the difference in their pricing strategies.

## Installation

To run this project, make sure you have Python installed. Additionally, you need to have the following libraries installed:

- Selenium
- BeautifulSoup
- pandas
- numpy
- matplotlib
- requests

You can install the required libraries using pip:

```bash
pip install selenium beautifulsoup4 pandas numpy matplotlib requests
```

You also need to have the appropriate web drivers for Selenium. The code uses Firefox as the browser. Download the latest version of the Firefox web driver from the official Mozilla website: https://github.com/mozilla/geckodriver/releases

Ensure that the downloaded executable is in the same directory as your Python script.

## Usage

The code is divided into two main sections: one for Mathem website scraping and the other for Hemkop website scraping. To run either part, comment out the code for the other part.

### Mathem Website Scraping

1. Import the required libraries at the beginning of your Python script.
2. Create a webdriver for Firefox using `webdriver.Firefox()`.
3. Use the `get()` function to navigate to the Mathem website's "extrapriser" page.
4. The script will scroll through the webpage and click on the "Next" button to load more products.
5. The data will be scraped, and a Pandas DataFrame will be created containing product names, original prices, and sales prices.

### Hemkop Website Scraping

1. Import the required libraries at the beginning of your Python script.
2. Create a webdriver for Firefox using `webdriver.Firefox()`.
3. Use the `get()` function to navigate to the Hemkop website's "veckans-erbjudanden" page.
4. The script will scroll through the webpage to load all products.
5. The data will be scraped, and a Pandas DataFrame will be created containing product names, original prices, and sales prices.

## Data Cleaning

Both Mathem and Hemkop data are cleaned by removing unwanted characters, converting prices to float values, and calculating the percentage saved for each product.

## Data Analysis

The project includes data analysis on the extracted data, such as plotting mean percentage savings for price groups and counting the number of products in percentage savings bins.

## NLP for Categorization

The project also includes an attempt at using Natural Language Processing (NLP) techniques to categorize product names.

Please note that web scraping may be subject to website terms of service, and you should use it responsibly and ethically.

## License

This project is licensed under the MIT License. Feel free to use and modify it according to your needs.

For additional support or questions, contact [your email or preferred contact method].
