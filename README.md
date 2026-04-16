# Project Name: World Population Web Scraper

## 1. Project Overview
* **Target Website:** https://www.worldometers.info/world-population/population-by-country/
* **Data Fields Extracted:** Country, Population, Yearly Change, Net Change, Density, World Share
* **Tools Used:** Python, requests, BeautifulSoup, pandas, matplotlib, time
This project scrapes real-time population data of countries from Worldometer and converts it into a structured dataset for analysis and visualization.

## 2. Setup Instructions
1. Clone this repo:
git clone https://github.com/mahamrizwan/web-scraping-assignment.git
2. Install dependencies:
pip install -r requirements.txt
3. Run the project:
Open the notebook file `webscraping.ipynb` in Google Colab or Jupyter Notebook and run all cells in order.

## 3. Challenges & Solutions
* One challenge was identifying the correct HTML table from multiple tables on the webpage. This was solved by selecting the largest table using BeautifulSoup.
* Another issue was that numeric values were stored as strings with commas, which affected sorting. This was fixed by cleaning the data and converting columns to integer format.
* There was also an encoding issue where special characters appeared incorrectly (e.g., â instead of -). This was resolved using string replacement during data cleaning.
* Finally, time delays were added using `time.sleep(1)` to follow ethical scraping practices and avoid overloading the website server.

## 4. Output Files
* population_data.csv → raw scraped data  
* population_clean (3).csv → cleaned dataset  
* webscraping.ipynb → main project notebook  
* requirements.txt → required libraries  

## 5. Notes
This project demonstrates web scraping, data cleaning, and basic data visualization using Python. The dataset is further analyzed by sorting and plotting the top 10 most populated countries.
