# Email_collector
This is a basic web scraping application to extract email addresses from websites. It takes a starting URL as input and crawls the website pages to find email IDs.
# Functionality
The key functions of the app are:
* Takes a starting URL as input through the GUI
* Performs a breadth-first search crawl of pages on the domain
* Scrapes each page for email addresses using regular expressions
* Emails are validated before saving
* Results are displayed in a GUI pop-up
E* mails are stored in a pandas DataFrame
# Usage
The app requirements are:
* Python 3
* Tkinter for GUI
* Requests and BeautifulSoup for web scraping
* Pandas for data storage
# To run the app:

python app.py

Input a starting URL of a website and click Extract Emails. Wait for the crawling and scraping to complete. If emails are found, they will be displayed in the result pop-up.

# Implementation
The main logic is in fetch_emails():
* Queue-based BFS crawl of website pages
* Scrape page with BeautifulSoup
* Regex to find email addresses
* Store valid emails in a DataFrame
* Repeat for all pages in crawl
* The GUI provides the textbox for input URL and displays the final result pop-up.
# Scope for Improvement
Some ways the app could be improved:
* Add depth limit for crawler
* GUI updates during processing
* Export emails to CSV/Excel
* Customizable email regexes
* Threaded scraping for better performance


Overall this provides a simple CLI tool for email scraping of a website using Python. More validation, error checking and features could be added to make it production-ready.
