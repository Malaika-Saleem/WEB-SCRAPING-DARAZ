Daraz.pk Product Scraper
This Python script utilizes Selenium to scrape product details from Daraz.pk, focusing on Redmi Note 12. The script extracts information such as product descriptions, prices, ratings, and seller details. The data is organized into a Pandas dataframe, and a scoring mechanism is applied based on ratings, seller ratings, on-time ratings, prices, free shipping, and Daraz Mall status. The highest-scoring product is identified and displayed.

Script Overview
Importing Libraries: The script starts by importing necessary libraries for web scraping, including Selenium, Pandas, and NumPy.

Setting Up WebDriver: Chrome WebDriver is initialized using the webdriver module from Selenium, and the Daraz.pk website is opened.

Data Extraction: Product details such as descriptions, prices, ratings, seller details, and more are extracted from each product card on the Daraz.pk search results page.

Organizing Data: The extracted information is stored in a dictionary called data, which is then converted into a Pandas dataframe. The dataframe is saved as a CSV file named Q3_data.csv after processing each page.

Scoring Mechanism: The script reads the saved CSV, calculates a score for each product based on predefined formulas, and updates the dataframe with the calculated scores.

Identifying the Best Product: The product with the highest score is identified and displayed as the best product. Additionally, the description of the product with index 40 in the dataframe is printed.
