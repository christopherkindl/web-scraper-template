# Turn Website Data into Analyse-Ready Datasets

Template based on `BeautifulSoup4` (HTML scraper) to scrape ads/listings from search-based platforms, such as property websites. 

![alt text](https://github.com/christopherkindl/web-scraper-template/blob/main/00_images/framework.png)

1. How to get one data point for one feature?
(e.g. get the price tag from the first ad)

2. How to get all data points for one feature from the entire page?
(e.g. get price tags of all ads on page)

3. How to get all data points for one feature available across all results pages?
(e.g. get price tags of every ad shown for a particular search request)

4. How to tackle inconsistency if the data point of interest is not always applicable in an ad?
(e.g. there are some ads in which price field says "Price on application". We would end up having a column consisting of numeric and string values which does not allow a ready-to-go analysis in our case. Of course, we could simply exclude string values when doing the analysis. This step is just to demonstrate how to anticipate a cleaner dataset from the beginning on which might be even more valuable in other cases)

5. How to better extract complex information?
(e.g. assume every ad contains public transportation information, such as "0.5 miles to subway station XY". What does the logic need to look like so that we can store this mix of information directly in the right format: distance = [0.5], transport_type = ["underground"], station = ["name XY"])

## Installation

Open your terminal and clone the repository:

```Shell
$ git clone https://github.com/christopherkindl/web-scraper-template.git
```

Install non-standard Python libraries:

```Shell
$ pip install -r requirements.txt
```
