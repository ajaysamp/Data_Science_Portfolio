# Data Wrangling and Cleaning

Data for the analysis was obtained from the ratebeer.com website.  The methods used for obtaining the data, cleaning and getting the data suitable for analysis are discussed in the subsequent sections.

# RateBeer Website

RateBeer.com is widely recognized as the most in-depth, accurate, and one of the most-visited source for beer information. RateBeer is a world site for craft beer enthusiasts and is dedicated to serving the entire craft beer community through beer education, promotion and outreach. Established and maintained by dedicated volunteers, RateBeer has become the premier resource for consumer-driven beer ratings, features on beer culture and industry events, weekly beer-related editorials, and an internationally recognized, annual RateBeer Best competition. A vibrant community of hundreds of thousands of members from more than 100 countries have rated hundreds of thousands of different beers around the world.

# Data Acquisition

The ratebeer website provides an API key for beer enthusiasts who are interested in developing beer apps in partnership with the website and for students who are interested in general data analysis research. For this project, an API key was obtained under the academia agreement with RateBeer.
The API documentation is provided at this link: https://www.ratebeer.com/api-documentation.asp.The data can be downloaded using the API key as json files. The data can be downloaded by ratings, 100 beers a time. A total of 5,000 calls are allowed per month. A for loop was written in python to do 100 calls at a time to avoid overloading the server. The details for data acquisition are provided in this ipython notebook.

# Data Cleaning

The dataset contains 220,000 beers from around the world. Each beer has 18 variables associated with it such as id, description, abv, name, style, style score, overall score, brewery name, brewery type, rating count, average rating, street, city, state, country, continent, twitter link, Facebook link and more. 
The cleaning process involved primarily inspecting and filling the missing values in the required columns. The columns such as beer description, street, city and continent were dropped during the cleaning process. The 'beer_description' column would have been interesting to look at from a sentiment analysis perspective or NLP. This will be something that will be considered for future work. The city and street columns were dropped since the analysis does not require that level of granularity. Binary columns for social media were created to analyze the influence on average ratings. 
The missing values in the numerical columns were coded as zero values. A detailed description of the data cleaning process is available in this ipython notebook.



