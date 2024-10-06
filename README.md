# Google News Scraper

This Python script scrapes news articles from Google News based on a search term provided by the user. It fetches the news in **RSS format**, extracts the titles and links of the articles, and stores them in an Excel file for easy access and analysis. The script is ideal for users looking to quickly retrieve and organize the latest news articles related to a specific keyword.

## Key Features
- **Customizable Search**: Users can input a keyword and specify the number of articles they want to scrape.
- **RSS Parsing**: The script retrieves news articles in RSS format using Google News' RSS feed.
- **Excel Export**: The results are saved in an organized Excel file containing the article titles and their corresponding links.

## How it Works
1. **Input**: The user provides a keyword to search for and the number of articles to fetch.
2. **RSS Feed Fetching**: The script sends a request to Google News RSS for the keyword.
3. **XML Parsing**: It parses the XML response to extract the titles and links of the news articles.
4. **Excel Output**: The data is saved in an Excel file with two columns: "title" and "links".

## Requirements
- Python 3.x
- `requests`
- `pandas`

Install the dependencies using:
```bash
pip install requests pandas
```

## How to Use
1. Run the script: `python google_news_scraper.py`
2. Provide the keyword and number of articles when prompted.
3. The output will be saved in an Excel file named `<keyword>_news_scrapper.xlsx`.

### Example
- **Input**: `Enter the news title keyword: technology`
- **Output**: An Excel file named `technology_news_scrapper.xlsx` with the latest news about "technology."

---

**Note**: Google News RSS feed might have limitations on the number of results or rate of access, so use this script responsibly.
