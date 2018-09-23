# Abstract

_Ajay Sampath_ 

_September 23, 2018_

Twitter is one of the most popular social media platforms in the world. The simple, but effective sharing channel has insights from 83% of the world’s leaders, 330 million monthly users and 3 billion account holders. 

It is no surprise so many companies want to tap into the potential of Twitter for their own social strategies. The fast-paced nature of this platform means that it’s a great way for brands to start building a strong online presence. Tracking twitter metrics could help make insightful decisions about future marketing campaigns. 

This project analyses tweets from the United States on one day. The primary purpose of the project is to understand how to scrape twitter, collect data and synthesis meaningful insights from the data. There are several future use cases for more specific tweet analytics and prior knowledge will help deliver solutions efficiently for existing and potential clients. 


# Data 

Data was scraped from twitter using the TwitteR package.  This is a R package that scrapes data from the twitter website. The biggest challenge in scraping the website is the rate limit – Twitter allows you to collect only 18,000 every 15 minutes. The R script mentioned before was run for 24 hours to collect a total of 1.7 million tweets. The tweets were limited for the English language and within the United States. The script was paused for 15 minutes as soon as the number of tweets reached 18,000. Luckily the system did not crash while collecting the data. 

Below is a list of variables that have been used for the analysis:

retweet_text: the text of original tweet that was retweeted<br>
retweet_source: device used for the original tweet that was retweeted<br>
retweet_favorite_count: number of likes for the original tweet was retweeted<br>
retweet_retweet_count: number of retweets for the original tweet that was retweeted<br>
retweet_followers_count: number of followers for the user with the original tweet that was retweeted<br> 
retweet_friends_count: number of users followed by the user with the original tweet that was retweeted<br>
retweet_statuses_count : number of tweets the original user has posted<br>
retweet_location: geographical location from where the tweeter posted the source tweet<br>
retweet_description: bio of the user with the source tweet<br>
retweet_verified: if the user with the original tweet is verified<br>

# Analysis Methodology

Typical exploratory data analysis methods have been applied to understand the tweet and user metrics. Relationships between the different metrics have also been explored and insights have been derived. Machine learning methods have been used to predict the favorites and retweet counts. NLP models have been applied to predict the target variables based only on the tweet text. 


# Deliverables

The following deliverables will be submitted as part of this project and will be made available in a git hub repository.
* Final Report/Paper - pdf
* Codes used for the analysis - ipython notebook

