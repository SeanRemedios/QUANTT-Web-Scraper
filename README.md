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

## License
MIT License

Copyright (c) 2019 Sean Remedios

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
