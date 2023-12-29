
# Web Scraping

This project allows me to extract the financial statements of every stock in the entire Thai Stock Market (SET). The end product of this project is approximately 600+ financial statements extracted, transformed, and loaded into a database.


## Acknowledgements

The initial URL used for scraping/crawling is: https://www.set.or.th/en/market/product/stock/search


## Project Diagram
![Screen Shot 2566-12-28 at 21 12 25](https://github.com/jarkthan/web-scraping/assets/93521945/f16092fb-cdea-4d3a-8dbd-ab48b283333b)

## Environment Setup
This project uses Google Chrome and Selenium, therefore a Chromedriver needs to be installed in the local computer prior to any coding. Pay attention to the local computer's Google Chrome version, the correct Chromedriver version must be installed for the specific Chrome version. 
- [Chromedriver](https://chromedriver.chromium.org/downloads)
The `requirement.txt` is also included in this repo. Use this following Bash command to create and download the environment packages required:
```bash
python3 -m venv <environment-name>
```
```bash
source <environment-name>/bin/activate
```
```bash
pip install -r requirements.txt
```

## How to Run the Program
`main.py` contains the main function which will trigger the whole program. Because the program could take up to 10 hours of running, it is decided to not scrape the industry group names (to check for new industry groups and new listed companies) everytime the program is run. So after running `main.py` two parameters should be asked, whether the user also wants to check for newly created industry and listed companies, or only to refresh the financial data of each stocks in the database.
```python
python main.py
```
