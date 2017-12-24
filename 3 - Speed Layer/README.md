# SPEED LAYER

## Description  
The task was to prepare speed layer computation based on some pre-processed streams of tweets.  
The data that should be used as for the streaming input is given in the twitter_ format.  
Each file represents a batch of data.  
We assume that each file contains *one hour* of streaming data.  
Each file holds a number of rows, each row is made of 7 fields:  
	- tweet ID,
	- creation date/time,
	- language of the tweet,
	- movie URL,
	- number of favourites,
	- number of retweets,
	- username.
	
## Task
We are interested in real-time monitoring of:  
	- knowing the popularity of each movie in the past, what is the average popularity of all movies that in one batch of data received engagement.  
	- the total engagement that is received per hour, by all movies.
	- the number of user tweets with and without engagement per user, per hour.  
Results are persisted in the Cassandra storage.  

## Streaming application  
1. Prepared the application to work with data stream that comes in.  
2. To not be affected by any data fluctuations, application uses last 2 batche for each batch computation (windows).  
3. Defined the streaming computation to calculate the average past popularity of movies tweeted about within an hour.  
4. Defined the streaming computation to get the total engagement received per hour.  
5. Defined the streaming computation to get the number of user tweets with and without engagement, per user, per hour.  

## Storing the results:  
1. Prepared Cassandra data structures to store the results of computations.  
2. Prepared code for writing the results of the computations into the Cassandra data structures.  

Rest of the explaination can be found in the code and the notebook.