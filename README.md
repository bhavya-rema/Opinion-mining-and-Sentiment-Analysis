# Opinion-mining-and-Sentiment-Analysis
Using POS-Tagging, create a parser for Hotel reviews To get Aspect opinion pairs and apply sentiment analysis on top.
Approach will be to find aspects of the hotels in the customer reviews and the sentiments associated with those aspects. 
Not using sentence level sentiment mining as there could be multiple sentiments in a single review.

## Procedure

1. Co reference resolution
2. Dependency Parsing
3. Creating Aspect opinion Pairs
4. Scoring aspect opinion for Positive or negative sentiments.
5. Aggregating sentiments scores on each aspect from multiple reviews for each hotel


![alt text](https://github.com/bhavya-rema/Opinion-mining-and-Sentiment-Analysis/blob/main/Aspect_mining.png)


![alt text](https://github.com/bhavya-rema/Opinion-mining-and-Sentiment-Analysis/blob/main/Sentiment_mining.png)

##### Example Statement
The room was pretty big and spacious.  It was clean.  The view was nice.

##### Co reference resolution
The room was pretty big and spacious.  The room was clean.  The view was nice.

##### Aspect opinion pairs
[('room', 'pretty big and spacious'), ('room', 'clean'), ('view', 'nice')]

##### Sentiment scores:
###### room Positive 0.4939
###### room Positive 0.4019
###### view Positive 0.4215
