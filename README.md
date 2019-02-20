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

## Automatically Run
To automatically run the program everyday, this can be done in two ways:
1. Crontab <br>
- Open a terminal window <br>
- Open the crontab file by entering the following command: <br>
```
crontab -e
```
- Enter the following command to run the program every Monday-FRIDAY AT 6pm EST:
```
* 18 * * 1-5 python2.7 webscraper.py <Quantopian Email> <Quantopian Password> <Google Sheets Link>
```
Note: The program will only run if your computer is on at 6pm. <br>

2. Contact the owner of the repository to have it uploaded to a server.

Note: A client_secret.json file is needed to run the program. This file can be obtained in two ways:
1. Contact the creator of the repository
2. Generate your own client_secret.json:
```
- Go to the Google APIs Console - https://console.developers.google.com/.
- Create a new project.
- Click Enable API. Search for and enable the Google Drive API.
- Create credentials for a Web Server to access Application Data.
- Name the service account and grant it a Project Role of Editor.
- Download the JSON file.
- Copy the JSON file to your code directory and rename it to client_secret.json
```
Note: To use the the client_secret.json supplied by the creator of the repository, share the Google Sheets with them as well.

## License
MIT License

Copyright (c) 2019 Sean Remedios
