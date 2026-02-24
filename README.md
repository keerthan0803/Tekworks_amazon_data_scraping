# Amazon Laptop Data Scraper

A Python-based web scraping project that extracts laptop product information from Amazon India and saves it to a CSV file for analysis.

## 📋 Description

This project scrapes laptop listings from Amazon India and extracts key product details including title, price, brand, RAM, storage, processor, ratings, and more. The data is then organized into a structured format and exported as a CSV file.

## ✨ Features

- Scrapes multiple pages of Amazon laptop listings
- Extracts detailed product information:
  - Product title
  - Price
  - Brand name
  - RAM capacity
  - Storage (SSD/NVMe)
  - Processor details (Intel Core series)
  - Windows version
  - Product color
  - Customer ratings
- Exports data to CSV format for easy analysis
- Uses regex for intelligent data extraction

## 🛠️ Technologies Used

- **Python 3.x**
- **BeautifulSoup4** - HTML parsing and web scraping
- **Requests** - HTTP requests
- **Pandas** - Data manipulation and CSV export
- **Regular Expressions (re)** - Pattern matching for data extraction

## 📦 Installation

1. Clone this repository:
```bash
git clone https://github.com/yourusername/amazon-laptop-scraper.git
cd amazon-laptop-scraper
```

2. Install required packages:
```bash
pip install beautifulsoup4 pandas requests
```

## 🚀 Usage

1. Open the Jupyter notebook:
```bash
jupyter notebook amazon_data_featching.ipynb
```

2. Run all cells in the notebook sequentially

3. The scraper will fetch data from 4 pages of Amazon laptop listings

4. Output will be saved as `amazon_laptops.csv` in the same directory

## 📊 Output Format

The CSV file contains the following columns:

| Column | Description |
|--------|-------------|
| Title | Full product title |
| Price | Product price (in INR) |
| Brand | Laptop brand name |
| RAM | RAM capacity |
| Rating | Customer rating |
| Storage | Storage capacity (SSD/NVMe) |
| Windows | Windows version |
| Color | Product color |
| Processor | Processor details |

## 📝 Requirements

```
beautifulsoup4
pandas
requests
```

## ⚠️ Important Notes

- This scraper uses appropriate headers to avoid being blocked
- Scraping should be done responsibly and in accordance with Amazon's Terms of Service
- The structure of Amazon's website may change, which could affect the scraper's functionality
- Consider adding delays between requests to avoid overwhelming the server

## 🔧 Customization

You can modify the following parameters in the notebook:

- **Number of pages**: Change the range in `for page in range(1, 5):`
- **Search query**: Modify the `params` dictionary to search for different products
- **Data fields**: Add or remove fields in the data extraction logic

## 📄 License

This project is open source and available for educational purposes.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the issues page.

## 👤 Author

Your Name
- GitHub: [@yourusername](https://github.com/yourusername)

## 🌟 Show your support

Give a ⭐️ if this project helped you!

---

**Disclaimer**: This project is for educational purposes only. Please ensure you comply with Amazon's Terms of Service and robots.txt file when scraping data.
