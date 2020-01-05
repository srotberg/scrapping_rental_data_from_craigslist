# Scraping Rental Data From Craigslist

This [code](scraping_example.py) scrapes rental data from Craigslist. For a given url, it scrapes all the listings of that area and produces a .csv file with rents, number of bedrooms, location, GPS coordinates, and distance to downtown.

Note that if the code loops over thousands of listings, this may take about 5-10 minutes to execute.

Then, it generates various statistics by the number of bedrooms as well as regresses rent on bedrooms and distance to downtown. 

Lastly, if you run this plotting [script](heat_map_example.py), you will get a heat map of all the rents around the city. Here is what I got when I ran the code on January 5th 2020:

<img src="heat_map_toronto_craigslist_data.png"/>

You will need these packages:
* requests
* BeautifulSoup
* pandas
* numpy
* geopy
* sklearn
* statsmodels
* seaborn
