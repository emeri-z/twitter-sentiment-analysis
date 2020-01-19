# twitter-sentiment-analysis

In this project, I analyzed POTUS's tweet behavior.

### Introduction
In this project, I analyzed POTUS's tweet behavior. I do the following: 
* **Data Import and Cleaning**: Import Donald Trump’s tweets (@realdonaldtrump) and convert from raw JSON to tidy Pandas DataFrame in Jupyter Notebook
* **EDA**: Conduct EDA, analyzing tweet sources and user behavior across devices and usage by time
* **Sentiment Analysis**: Implement sentiment analysis to calculate tweet polarity distributions using the VADER  (Valence Aware Dictionary and Sentiment Reasoner) lexicon. I look at overall sentiment, polarity around key election and inauguration dates, mentions of “fake news”, and differences in sentiment distribution over keyword pairs and tweets with and without hashtags. Finally, for the most retweeted tweets, I find the retweet count and top 20 keywords.

Files:
* *Trump-Twitter-Text.ipynb*: all code
* *hw4-realdonaldtrump_tweets.json*: all data
* *vader_lexicon.txt*: used for sentiment analysis


### Analysis and Results


### Future work:


1. I have scraped Tweets with tweepy and Twitter’s API before, and I have included code in “twitter_scrape.ipynb”. I hope to repeat this analysis on more recent tweets, particularly as rumors and memes of WWIII circulate the internet. 
2. This is a really amazing interactive article by the NYTimes. In the future, I hope to be able to create something of the sort: https://www.nytimes.com/interactive/2019/11/02/us/politics/trump-twitter-presidency.html
3. I could dive deeper into the history of Trump’s presidencies, aligning real-word events and media releases with the sentiment of his Tweets.
4. For a more ML geared approach, I can extend this by building a Naive Bayes Classifier.

I am always open to feedback; feel free to ping me @emeri.zhang@berkeley.edu! I will push as I make updates to this project.
