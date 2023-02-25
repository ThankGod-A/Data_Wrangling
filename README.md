### Data_Wrangling

#### Introduction
The project I am working on is on Data Wrangling and the dataset that I will be wrangling (and analyzing and visualizing) is the tweet archive of Twitter user @dog_rates also known as WeRateDogs
WeRateDogs is a Twitter account that rates people's dogs with a humorous comment about the dog. These ratings almost always have a denominator of 10. The numerator is almost always greater than 10. 11/10, 12/10, 13/10, etc. The WeRateDogs dataset provided by Udacity consists of over 5000 records but is incomplete. The dataset does not include a Retweet count and Favorite (Like) count. In order to get the WeRateDogs Retweet and Like count, I queried this data off of Twitter using Tweepy to query Twitter's API for additional data beyond the data included in the WeRateDogs Twitter archive. This additional data included retweet count and favorite count.
This wrangling process involves three stages, namely: **Data Gathering** sometimes called acquiring or collecting data, **Data Assessing**, and **Data Cleaning**.

#### Data Gathering
A CSV file called ‘twitter-archive-enhanced.csv’ was downloaded manually and imported or loaded into my Jupyter notebook as Pandas DataFrame. A TSV file called ‘image-predictions.tsv’  was programmatically downloaded using the requests library, and read into Jupyter notebook as Pandas DataFrame using pd.read_csv function.
Lastly, I queried Twitter data using Tweepy. I created a for loop for each tweet_id in the twitter-archive-enhanced.csv, I then created an empty list and read the Json.txt file line by line into Pandas DataFrame with tweet_id, retweet_count, and favorite_count as variables.

#### Data Assessing
Here, the data were assessed both visually & programmatically for Quality and Tidiness issues. The issues discovered were dully documented.

#### Data Cleaning involves defining the issues discovered in the data assessment, Converting my definitions into executable code, and testing my data using code to ensure my code was implemented correctly.

#### Limitation
- The tweet status of thirty-one (31) users was missing from the dataset whilst querying Twitter data. 
- So many columns were redundant because they are either not necessary or they contain too much missing data.

#### Ps: The result of my analysis and visualization can be found in the Act_Report.html file while the Wrangling process can be found in the Wrangle_Project_2.ipynb file.
