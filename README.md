# Tesla Stock Data Scraper

This project is a Python-based web scraper that collects Tesla's yearly and quarterly revenue data from online financial sources. Using libraries like Selenium, BeautifulSoup, and pandas, it automates the data extraction process, organizes the revenue data, and outputs it into a structured format (e.g., CSV or Excel) for further analysis.

## Features

- **Automated Web Scraping**: Uses Selenium and BeautifulSoup to automate the data extraction process.
- **Data Organization**: Collects and formats both yearly and quarterly revenue data for Tesla.
- **Export Options**: Saves the collected data as a CSV or Excel file for easy access and analysis.

## Prerequisites

To run this project, you will need:

- **Python 3.7+**
- **WebDriver**: Compatible with the browser you will use (e.g., ChromeDriver for Chrome).
- **Libraries**:
  - Selenium
  - BeautifulSoup
  - pandas

Install the required libraries using:
```bash
pip install selenium beautifulsoup4 pandas
```

## Project Structure

- scraper.py: The main script for running the web scraping logic.
- config.py: Configures the URL and parameters used for web scraping.
d- ata/: Directory where the collected data (CSV/Excel) will be stored.


## Usage

1. **Set Up WebDriver**:
   - Download the appropriate WebDriver for your browser (e.g., ChromeDriver for Chrome) and place it in your PATH or specify its path in `scraper.py`.

2. **Configure the URL and Selectors**:
   - Modify `config.py` to set the URL of the site containing Tesla's revenue data and update selectors if needed.

3. **Run the Scraper**:
   ```bash
   python scraper.py
   ```

## Sample Output

The output file will contain columns such as:

    Year
    Quarter (if quarterly data)
    Revenue
    Timestamp (date and time of data extraction)
