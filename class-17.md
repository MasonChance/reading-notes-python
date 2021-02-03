# Web-Scraping Basics
web scraping is the art and science of using a script to pull large amounts of data from a website based on pre-planned criteria, and then downloading that data into a useable format automatically. One usually begins the process of developing a scraper for a specific type of data, by identifying where on the website or group of similarily designed websites, the links to that data are located. It is from here that the real work begins. 

imports:
```
  import requests
  import urllib.request
  import time
  from bs4 import BeautifulSoup

```

much like in JavaScript Python has a requests library for handling server request and response protocols. by passing the url to this request/response protocol we can access the data available there. the data that comes back will inherently be messy and difficult to read, to make this a little easier we can use the [BeautifulSoupl library](https://www.crummy.com/software/BeautifulSoup/bs4/doc/) to parse the HTML and make it a little more readable for lowly humans such as ourselves. The return of Beautiful soup parsing is a data structure similiar to a pandas dataframe and the individual attributes are accessed in much the same way. 
the example below is taken from the article [How to Web Scrape with Python in 4 Minutes: by Julia Kho](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)
```
one_a_tag = soup.findAll(‘a’)[38]  # the variable `one_a_tag` becomes a dataframe object of the anchor tags *html* from our initial parsing and we access it at the 38th index *indicated by the square brackets*

link = one_a_tag[‘href’]   # now we have a series object and we access it at it's <href> attribute again using bracket notation. 

```

we then use the urllib library to compose the full locate, access, name-file, and download file sequence. 

It is important to note, especially when intending to download large amounts of data, that peoples servers get upset when they get an unusual ammount of requests rapidly, as it bogs down the server and can cause issues for their users on the site. in writing our script it is important to review the ToS for the site we intend to scrape and make sure we are following both legal and conventional guidelines for site use. 

to avoid getting flagged as spam and limit the workload imposed on the site we are scraping we can set an interval timer of sorts with the following line of code:
`time.sleep(time_in_seconds)`. different ToS may have different requirments and it's important to make sure to set the timer accordingly. 






#### [Return to Main index of Notes](./README.md)