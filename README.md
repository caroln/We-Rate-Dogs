# We Rate Dogs
## Carolyn Cherono


## We Rate Dogs

This project wrangled, analyzed and visualized the tweet archive of Twitter user @@dog_rates, also known as WeRateDogs. WeRateDogs is a twitter account that rates people's dogs with a humorous comment.


## Steps

 Gather Data
Twitter_archive_enhanced.csv was Provided by Udacity and was loaded into a dataframe called ‘archive’
Image_predictions.tsv was downloaded programmatically using Requests and was loaded into a dataframe called ‘image_pred’
Additional data such as favorite and retweet_count was gathered by usingTweepy API and stored in a ‘tweet_json.txt’ file and data frame called ‘tweet_count’.
2 & 3 Assess and Clean
Remove tweets without images.
Remove tweets with retweet.
Remove unnecessary columns.
Convert non-dog names to 'None' then make title case.
The rating_numerator and rating_denominator have offbeat values.
Several columns have empty values, such as in_reply_to_status, in_reply_to_user_id, retweeted_status_id, retweeted_status_user_id, retweeted_status_timestamp.
Convert timestamp to datetime.
Change source column from ulr type to text.
Dog Stages into 1 column instead of 4.
The prediction column of dog breed can be simplified.
Join tweet_archive, image_prediction, tweet_json into one master dataset on tweetid.

## Requirements

Python
Numpy
Pandas
Matplotlib
requests
json
tweepy
datetime