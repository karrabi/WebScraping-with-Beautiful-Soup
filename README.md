# WebScraping-with-Beautiful-Soup
This project is about extracting **Top 10 Crypto** data from [Coin Market](https://coinmarketcap.com/coins/) website. 

Target webpage shows top 10 records during first load, then loads rest of records based on user page scroll. For loading all 100 records we should use [Selenium](https://www.selenium.dev/) but, i want to show how you can WebScraping with [Beautiful Soup](https://pypi.org/project/beautifulsoup4/) library, so for now, we are satisfied with these 10 records.

The code contains 3 steps:

1- ***lines 2 - 6***: Load the page and parse its content with BeautifulSoap

2- ***Line 7***: Navigate the data structure with *find_all* looking for all ***p*** tags with specific class names. 

The target data exists in a table so I easily extract the p tag's class-names with my browser inspector and write them in code. this way I extract each column of data separately.

3- ***Line 9 - 14***: Extract list of values from just extracted ***p*** and save them in a DataFrame Column.


Thats it. Very simple. Enjoy