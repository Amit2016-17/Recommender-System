# BATCH LAYER

## Description  
The task was to prepare the batch layer (off-line processing pipeline) of the lambada architecture used to perform social media analysis.  
The dataset used is MovieTweetings (https://github.com/sidooms/MovieTweetings) dataset which is a snapshot of tweeets of IMDb activities of users who use its mobile app.  
Each tweet contains a number of fields that store information about the tweeet, user who tweeted, hashtags, URLs and the reactions of other users to tweets and other metadata.  

## Files  
Below are the files containing a subset of MovieTweetings dataset:  
	- Small: https://s3-eu-west-1.amazonaws.com/jwasilewski/twitter.small
	- Medium: https://s3-eu-west-1.amazonaws.com/jwasilewski/twitter.medium
	
## Tasks  
1. Tweets-oriented analyses:  
	- number of tweets per day, per month, per year.
	- number of tweets with interactions (favourites + retweets) per day, per month, per year.  

2. Movies-oriented analyses:  
	- number of tweets about every single movie, per day and per month.  
	- amount of interactions a movie receives (favourites + retweets).  
	- popularity of each movie among different language-speakers.  
	
3. Users-oriented analyses:  
	- number of followers, favourites, statuses and listings of all users.  
	
## Advanced Analyses  
1. What are the top 20 most popular movies?  
2. In whihc month we collected the most interactions?  
3. What is the most popular movie in the group of Spanish-speaking users?  
4. What are the users with the most changes in number of followers between first and last tweet?