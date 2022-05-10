# Class 17
## Reading

### [Web Scrape with Python in 4 minutes](https://towardsdatascience.com/how-to-web-scrape-with-python-in-4-minutes-bc49186a8460)
- Web scraping is a technique to automatically access and extract large amounts of information from a website
- Read through the website’s Terms and Conditions to understand how you can legally use the data
- Most sites prohibit you from using the data for commercial purposes
- Make sure you are not downloading data at too rapid a rate because this may break the website
- Start by importing the following libraries:

      import requests
      import urllib.request
      import time
      from bs4 import BeautifulSoup
- Next, we set the url to the website and access the site with our requests library.

      url = 'http://web.mta.info/developers/turnstile.html'
      response = requests.get(url)
- Next we parse the html with BeautifulSoup so that we can work with a nicer, nested BeautifulSoup data structure

      soup = BeautifulSoup(response.text, “html.parser”)
- We use the method .findAll to locate all of our \<a> tags.

      soup.findAll('a')
- Next, let’s extract the actual link that we want. Let’s test out the first link.

      one_a_tag = soup.findAll(‘a’)[38]
      link = one_a_tag[‘href’]
- Last but not least, we should include this line of code so that we can pause our code for a second so that we are not spamming the website with requests
   
      time.sleep(1)

### [What is Web Scraping?](https://en.wikipedia.org/wiki/Web_scraping)
* web crawling is a main component of web scraping, to fetch pages for later processing
* There are methods that some websites use to prevent web scraping, such as detecting and disallowing bots from crawling (viewing) their pages
* In response, there are web scraping systems that rely on using techniques in DOM parsing, computer vision and natural language processing to simulate human browsing
### [How to scrape websites without getting blocked](https://www.scrapehero.com/how-to-prevent-getting-blacklisted-while-scraping/)
* The robot.txt filehas specific rules for good behavior, such as how frequently you can scrape, which pages allow scraping, and which ones you can’t
* If you need some data that is forbidden by Robots.txt. You could still scrape it
* Here are a few easy giveaways that you are bot/scraper/crawler –

      Scraping too fast and too many pages, faster than a human ever can
      Following the same pattern while crawling. For example – go through all pages of search results, and go to each result only after grabbing links to them. No human ever does that.
      Too many requests from the same IP address in a very short time
      Not identifying as a popular browser. You can do this by specifying a ‘User-Agent’.
      using a user agent string of a very old browser
* Incorporate some random clicks on the page, mouse movements and random actions that will make a spider look like a human.
* Create a pool of IPs that you can use and use random ones for each request
* Along with this, you have to spread a handful of requests across multiple IPs.
## Videos
* This youtuber made a scraper to track the price on a camera on Amazon
* Find any html element on a page by id using soup
* Use google two-step verification to make email protocol
### [Track Amazon Prices](https://www.youtube.com/watch?v=Bg9r_yLk7VY)
## Bookmark and Review
[Beautiful Soup](https://www.crummy.com/software/BeautifulSoup/)