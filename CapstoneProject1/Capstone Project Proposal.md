
# Abstract

_Ajay Sampath_ 

_January 11, 2018_


This project will analyze beer ratings from all around the world. The idea is to understand which countries have the most popular beers and the parameters affecting the ratings. The project will also look at the beers from the United Stated to find the cities with the best beers. 

Beers are the most popular drink in the world and mostly the preferred drink during celeberations, especially in the United States. It will be interesting to look at some of the key questions as below:

* Which country and city in the US has the most popular beers?
* Does the type brewery (micro, commercial etc.) affect the ratings?
* Does having a social media account help get better ratings?
* What other factors affect the ratings? Type of beer? No. of Ratings? 

The project will apply machine learning techniques to predict beer ratings given a set of known parameters. 

**_Who will be interested?_**

This will be interesting for a wide range of audience. Beer fans will be curious to see if there are drinking the right beers or think about trying something new! Restaurant owners and bars can stock beers according to the popularity of the beers. Breweries will get insights into the style of beer they need to focus on or if it will be worthwhile to invest in social media marketing. 

<img style="float: left;" src="beer.jpg"/>


# Data 

Data will be obtained from the website ratebeer.com. They have a developer API and give access to their data. The data can also be explored on a graphiql interface, though limited. A curl script with a python wrapper will be required to download the data in a json format. At any given point in time you can download data for 100 beers and a total of 5000 API calls are allowed per month. The total expected number of beers is 500,000. 

The following attributes are available:
* beer_id
* beer_name 
* beer_description
* beer_abv
* beer_StyleScore
* beer_AverageRating
* beer_ratingCount
* beer_style
* brewery_name
* brewery_type
* brewery_sity
* brewery_state
* brewery_country
* brewery_continent
* brewery_twitter
* brewery_facebook

From a preliminary review of the dataset, it looks like there are missing values for the geographical location and the social media attributes. Most likely, these values will have to be filled-in depending on the brewery name using a different database. There are no missing values for the other fields. 

# Analysis Methodology

The biggest challenge will be is to fill in the missing values for the geographical locations and the social media attributes. Preliminary search on the internet indicates that there is no existing database with this information. An independent database has to be created manually, which can be time consuming.

One of the challenges can be is that the ratings can be biased. For example, a person from Belgium may likely tend to rate a beer from their home country slightly higher. Also, the ratings can depend significantly on the mood of the person. However, since we have no control or information on this, we need to assume people were true to the ratings. Also, there are only three numerical variables in the dataset and the rest are categorical, which can be challenging for prediction analysis.

The effect of different attributes such as abv, rating count, beer style, brewery type and location on ratings will be analyzed independently. Summary statistics will be analyzed and plotted for the different attributes. Machine learning techniques (regression analysis) will be applied to predict the ratings for the beer. This can also be treated as a classification problem if we want to predict the country of the beer. This will be done if time permits. 


# Deliverables

The following deliverables will be submitted as part of this project and will be made available in a git hub repository.
* Final Report/Paper
* Presentation
* Codes used for the analysis
