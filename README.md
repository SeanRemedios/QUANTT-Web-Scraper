# QUANTT-Web-Scraper
This web scraper program is for the QUANTT team at Queen's University to scrape Quantopian in order to get data on each live trading algorithm.

## How to use
1. Install the requirements
```
pip install -r requirements.txt
```
2. Share the Google Spreadsheet with the following email address, giving it editing privilges
```
quantt-web-scraper@quantt.iam.gserviceaccount.com
```
3. Run the program. Copy and paste the URL directly from the browser as the 3rd argument
```
python2.7 webscraper.py <Quantopian Email> <Quantopian Password> <Google Sheets Link>
```

Note: A client_secret.json file is needed to run the program. This file can be obtained in two ways:
1. Contact the creator of the repository
2. Generate your own by going to https://console.cloud.google.com/, creating a new project, enabling Google Drive and Google Sheets API and downloading the credentials for a web application.
