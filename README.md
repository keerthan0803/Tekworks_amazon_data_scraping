# Amazon Laptop Data Scraping Project

## Overview
This project scrapes laptop data from Amazon India using web scraping techniques and performs data cleaning and analysis. The goal is to extract laptop specifications and pricing information for further analysis.

## Project Structure

### Files

1. **amazon_scraping.ipynb**
   - Main web scraping notebook
   - Extracts laptop data from Amazon India search results
   - Uses BeautifulSoup and Requests libraries for scraping
   - Collects raw product data including titles, prices, and ratings

2. **cleaning_scraped_data.ipynb**
   - Data cleaning and preprocessing notebook
   - Removes duplicates and invalid rows
   - Fills missing values using statistical methods (mode)
   - Standardizes price data format
   - Outputs cleaned dataset to `amazon_laptop_cleaned.csv`

3. **analysis_report.ipynb**
   - Exploratory Data Analysis (EDA) notebook
   - Generates insights and visualizations
   - Analyzes pricing, specifications, and ratings

4. **amazon_laptop_raw.csv**
   - Raw scraped data (before cleaning)
   - Contains all extracted laptop information with potential duplicates and missing values

5. **amazon_laptop_cleaned.csv**
   - Cleaned and preprocessed data
   - Ready for analysis and modeling

## Data Fields Extracted

- **Product Title**: Laptop model and name
- **Brand**: Laptop manufacturer (Apple, Dell, HP, Lenovo, Asus, etc.)
- **Processor**: CPU information (Intel Core i3/i5/i7/i9, AMD Ryzen, Apple M1/M2/M3)
- **RAM**: Memory size in GB
- **Storage (SSD)**: Storage capacity and type
- **Windows Version**: Operating system version (Windows 10, 11, etc.)
- **Color**: Available color options
- **Price**: Laptop price in INR
- **Rating**: Customer rating (0-5 stars)

## Dependencies

```
pandas
numpy
requests
beautifulsoup4
```

## How to Use

1. **Run Web Scraping**
   - Execute `amazon_scraping.ipynb` to scrape fresh data from Amazon
   - Results are saved to `amazon_laptop_raw.csv`

2. **Clean the Data**
   - Run `cleaning_scraped_data.ipynb` to process and clean the raw data
   - Outputs `amazon_laptop_cleaned.csv`

3. **Analyze the Data**
   - Open `analysis_report.ipynb` to explore insights and visualizations

## Data Cleaning Process

- Remove invalid/duplicate rows
- Handle missing values in specifications (RAM, Storage, Processor)
- Standardize price format (remove commas, convert to numeric)
- Drop unnecessary columns (Windows version)
- Reset index for consistency

## Notes

- Web scraping respects Amazon's terms of service and uses appropriate headers
- Missing values are filled with the mode (most common value) from each column
- Price data is converted to numeric format for analysis
- The dataset focuses on laptops available on Amazon India

## Future Enhancements

- Add more detailed product specifications
- Implement price tracking over time
- Add performance benchmarking data
- Create predictive models for laptop pricing
