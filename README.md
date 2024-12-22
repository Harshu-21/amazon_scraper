Documentation - Amazon Best Sellers Scraping Task 


1. Script Functionality
This Python script is designed to scrape Amazon's Best Sellers page and extract product details based on specific criteria:
1.	Authentication:
o	Logs into Amazon using user-provided credentials (email and password).
2.	Data Collection:
o	Scrapes the top 1500 best-selling products in 10 specified categories.
o	Collects data for products with discounts greater than 50%.
o	Extracted details include:
	Product Name
	Price
	Discount Percentage
	Rating
	Category Name
3.	Data Storage:
o	Saves the extracted data in a structured CSV format.
________________________________________
2. Setup Instructions
Step 1: Install Required Software
•	Python: Install Python 3.8 or higher. Verify with python --version.
•	Google Chrome: Ensure it's updated to version 131.0.6778.140.
•	ChromeDriver: Download the corresponding version of ChromeDriver from ChromeDriver Downloads.
•	Install Python Libraries: Use pip install selenium pandas.
Step 2: Prepare the Script
•	Update the Python script:
1.	Amazon Credentials: Replace placeholders for USERNAME and PASSWORD with your login credentials.
2.	ChromeDriver Path: Update the path to ChromeDriver in the script.
3.	Categories: Specify the categories to scrape in the CATEGORIES list.
________________________________________
3. Usage Guidelines
1.	Open the terminal and navigate to the folder with the script:
bash
Copy code
cd path/to/amazon_scraper
2.	Run the script:
bash
Copy code
python amazon_scraper.py
3.	The script will:
o	Log in to Amazon.
o	Scrape product details from specified categories.
o	Save the output as amazon_best_sellers.csv.
4.	Locate the CSV file in the script's directory.
________________________________________
4. Notes
1.	Error Handling: The script skips errors like CAPTCHAs or unresponsive pages and continues execution.
2.	Compliance: Use responsibly and adhere to Amazon’s terms of service.
3.	Future Updates: Update CSS selectors in the script if Amazon changes its website structure.
