# Web-Scraping-of-World-Atlas-Country-Data
Web Scraping of World Atlas: A Python-based data collection tool that extracts and saves country-specific information including names, flag images, and population figures into an easily accessible CSV format. #Python 

## 🪟 Overview:

This project focuses on web scraping techniques used to extract country-specific data from the World Atlas. The main objective of the project is to create a structured data set from the unstructured data available on the website, which can be further used for data analysis and visualization and perhaps to enrich other data sets.

## 🎯 Goals
- Extract country data, including names, images of national flags, and population figures.
- Store the extracted data in a Pandas DataFrame for manipulation.
- Save the structured data to a CSV file.

## ⚒️ Tools and Technologies
- **Python**: The primary programming language used for the project.
- **Requests**: A Python HTTP library used to send HTTP requests to the website.
- **BeautifulSoup**: A Python library for parsing HTML and XML documents and extracting data.
- **Pandas**: A powerful data manipulation tool used to create DataFrames and export the data to CSV format.

## 📊 Data
The data extracted from the World Atlas contains the following attributes for each country:
- **Country**: The name of the country.
- **Image**: The URL of the country's flag image.
- **Population**: The population of the country.

## 📎 Methodology
The `world_atlas_scraper.py` script performs the following actions:
- Send a GET request to the World Atlas country page.
- Parse the HTML response to find relevant country data.
- Iterate through each country element and extract the country name, flag image URL, and population.
- Handle any discrepancies in data type during extraction, particularly with population figures.
- Store the extracted data in a Pandas DataFrame.
- Export the DataFrame to a CSV file for easy access and distribution.

## 📃 Use

Before using the scraping script provided in this repository, ensure you perform the following steps to ensure it functions correctly:

1. **Modify the CSV Save Path**:
- The script includes a predefined path where the CSV file will be saved. **It is essential that you modify this path to match a directory** on your system where you have write permissions. Open the script and locate the line where the `to_csv` method is called, then replace the path with your own. For example:

     ```python
   csv_save_path = r'C:\Users\YourUsername\Documents\countries_data.csv'

