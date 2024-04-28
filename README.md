# Web-Scraping-of-World-Atlas-Country-Data
Web Scraping of World Atlas: A Python-based data collection tool that extracts and saves country-specific information including names, flag images, and population figures into an easily accessible CSV format. #Python 

## 🪟 Overview

This project focuses on web scraping techniques used to extract country-specific data from the World Atlas. The main objective of the project is to create a structured data set from the unstructured data available on the website, which can be further used for data analysis and visualization and perhaps to enrich other data sets.

[world_atlas_scraper.py](https://github.com/IrisMejuto/Web-Scraping-of-World-Atlas/blob/main/world_atlas_scraper.ipynb)
[CSV File]()
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

Before running the scraping script provided in this repository, make sure to perform the following essential step to ensure it functions correctly:

1. **Modify the CSV Save Path**: The script includes a specific line where the path for saving the CSV file is defined. You must modify this path to one that is valid on your own computer where you have the necessary write permissions. Locate the following line in the script:

   ```python
   # Save the DataFrame to a CSV file
   countries_df.to_csv(r'Z:\Programas\Anaconda\Notebooks\Proyectos propios\Wordl Analysis\countries_data.csv', index=False)


