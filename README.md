# Beergression - Predicting Brewery Scores on BeerAdvocate.com


## Introduction:
Given information from various web sources, is it possible to accurately predict a Brewery's score on [BeerAdvocate.com](https://www.beeradvocate.com). If so, which features are the most important in predicting such. The results of the models were scored based on their Adjusted r-squared.


## Tools:
* **BeautifulSoup4** - Data Gathering from various web sources
* **Python/Pandas** - Data Cleansing and feature engineering
* **Matplotlib/Seaborn** - Data Visualization


## Processes and Methods:
* Models - Ordinary Least Squares (OLS)
* Regularization Techniques:
    * Ridge 
    * LASSO
    * GridSearchCV
    * KFold Cross Validation


## Interesting Findings
* **Beer purists don't like eateries** - Significant negative correlation between a brewery's score and whether it was an eatery.
* **People like sours** - Not only do people appreciate a good sour (i.e. a brewery will have a higher score if they've produced a good sour) but they're more concerned with the quality (score) of a sour beer than the total number of sour beers. For sours - Quality over quantity.
* **People like IPAs and Pale Ales** - No surprise to anyone reading this but people like IPAs. However, unlike sours, the number of IPAs correlated more strongly to a brewery's score the quality (score) for those IPAs. For IPAs - Quantity over quality.
* **More is better** - Generally speaking, simply producing more beers is better for you brewery's score.
* **Good trumps bad** - While the max score by brewery for a particular style category or the simply the max score across all beers correlated significantly with a brewery's score, the respective minimum scores did not. What this ultimately conveys is that a brewery should not be partic ularly concerned with how beers that are flops and failures (i.e. low scoring beers) affect their brewery's score. Just focus on the positive!