# What is Web Scraping
Web scraping, web harvesting, or web data extraction is data scraping for extracting data from websites. 
Typically done using automated processes implemented using a bot or web crawler
Typically put into a database
It involves mostly fetching it and extracting from it
# how to web scrape with python
So once again you will be downloading data from a website
There are hundreds of .txt files exist on a site 
Those are what we are taking
It would be a pain to do it manually so that is why we are going to be web scraping
## Important things to know about Web Scraping
Read through the terms and conditions to see what you can actually do with the data
Make sure you are not downloading data at too rapid a rate because this may break the website. You may potentially be block from the site as well
# Inspecting the Website
First thing is we need to find the link to the files we watn to download inside the multiple levels of HTML tags
We want to find the relevant code on a website that contains our data
Inspect > Console will pop up > there is an arrow symbol > then click around on the website and it will show you the particular code associated with that part of the website
Python Code
Import the libraries import requests import urllib.requests import time
Then from bs4 import beautiful soup 
Then we set the url to the website and access the site with our requests library
Url = website url
Response = requests.get(url)
Id the access was successful you should see the following output
It should give you a response of 200
The we parse the html with beautiful soup so that we can work with a cleaner data structure
Soup = beautifulsoup(response.text, ‘html.parser’)
We use the method .findall to locate all of our <a> tags
soup.findAll(‘a’)
This code gives every line of code that starts with an <a> tag. The information that we are interested in starts at line 38 as seen below
Next we extract the actual link that we want. Let’s test out the first link
One_a_tag =soup.finAll(‘a’)[38]
Link = one_a_tag[‘href’]
The code saves the first text file
