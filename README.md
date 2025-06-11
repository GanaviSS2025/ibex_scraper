The task is to:
-Opens the IBEX electricity market webpage
-Collects 3 tables (prices, volumes, products)
-Cleans the data 
-Saves the data into Databricks tables so we can use it later

🧰 What tools does it use?
Selenium – to open the webpage like a real browser
BeautifulSoup – to read and extract tables from the page
PySpark – to create big data tables
Databricks – where we run everything and save the final data

🪜 Steps in the notebook:
-Install Chrome and Selenium
-Needed to open the website and read dynamic tables
-Start Spark
-Helps us work with big data easily
-Write helper functions
-One to clean number formats
-One to scrape and extract the tables
-Open the webpage
-Using Selenium and headless Chrome (no window)
-Extract 3 tables
-Each table has different data (daily, hourly, and product-based)
-Save tables into Databricks
-Stored as Delta Tables so we can use SQL to read them

📦 Output Tables
-Table Name	Description
-prices_volumes_table	Daily total volume and price info
-block_products_table	Prices for different energy products
-hourly_products_table	Hourly prices and volumes
