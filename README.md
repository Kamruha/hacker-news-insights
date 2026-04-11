Hacker News Scraper & Analyzer

A Python-based tool that collects, analyzes, and exports data from Hacker News.
The project demonstrates real-world web scraping, data processing, and report generation using clean and structured code.

Overview

This project automatically scrapes multiple pages from Hacker News and extracts key information about posts.
The collected data is processed, sorted, and exported into a well-formatted Excel file for further analysis.

The goal of this project is to simulate a real-world data pipeline:
data collection → data processing → data analysis → data export.

Features

* Scrapes multiple pages from Hacker News
* Extracts post title, link, author, time, score, and comments
* Handles missing data safely
* Converts text-based values into numeric format
* Sorts posts by number of comments
* Displays top-performing posts
* Exports results to a formatted Excel file
* Automatically adjusts column widths
* Applies basic styling for better readability

Technologies Used

* Python
* requests (HTTP requests)
* BeautifulSoup (HTML parsing)
* openpyxl (Excel file generation)

How It Works

1. The script sends HTTP requests to Hacker News pages
2. HTML content is parsed using BeautifulSoup
3. Each post is extracted along with its metadata
4. Data is cleaned and converted into usable formats
5. Results are stored in a structured list
6. Data is sorted based on engagement (comments)
7. Output is saved into an Excel file with formatting

Project Structure

* main script handles scraping, processing, and exporting
* data is stored in memory as a list of dictionaries
* Excel file is generated as the final output

Output Example

The generated Excel file contains:

* Title
* Link
* Author
* Time
* Score
* Comments

Posts are sorted by number of comments in descending order, making it easy to identify trending discussions.

Use Cases

* Market and trend analysis
* Monitoring popular discussions in tech
* Data collection for further analytics
* Portfolio demonstration of scraping skills

Installation

Install required dependencies:

pip install requests beautifulsoup4 openpyxl

Run

python your_script_name.py

Output file will be created in the project directory:

hacker_news.xlsx

Notes

* A delay between requests is used to avoid overloading the server
* The script is designed to handle missing or incomplete data gracefully
* The project focuses on clean structure and readability

Future Improvements

* Add data visualization (charts)
* Build a web interface (Streamlit or Flask)
* Implement async scraping for performance
* Add filtering and keyword search
* Store data in a database

Author

Developed as a practical project to demonstrate web scraping, data processing, and report generation skills.
