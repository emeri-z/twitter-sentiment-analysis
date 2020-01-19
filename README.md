# twitter-sentiment-analysis

In this project, I analyzed POTUS's tweet behavior.

### Introduction
In this project, I do the following: 
* **Data Import and Cleaning**: Import Donald Trump’s tweets (@realdonaldtrump) and convert from raw JSON to tidy Pandas DataFrame in Jupyter Notebook
* **EDA**: Conduct EDA, analyzing tweet sources and user behavior across devices and usage by time
* **Sentiment Analysis**: Implement sentiment analysis to calculate tweet polarity distributions using the VADER  (Valence Aware Dictionary and Sentiment Reasoner) lexicon. I look at overall sentiment, polarity around key election and inauguration dates, mentions of “fake news”, and differences in sentiment distribution over keyword pairs and tweets with and without hashtags. Finally, for the most retweeted tweets, I find the retweet count and top 20 keywords.

Files:
* [Trump-Twitter-Text.ipynb](https://github.com/emeri-z/twitter-sentiment-analysis/blob/master/Trump-Twitter-Text.ipynb): All code
* [hw4-realdonaldtrump_tweets.json](https://github.com/emeri-z/twitter-sentiment-analysis/blob/master/hw4-realdonaldtrump_tweets.json): all data 
* [vader_lexicon.txt](https://github.com/emeri-z/twitter-sentiment-analysis/blob/master/vader_lexicon.txt): used for sentiment analysis


### Analysis and Results

EDA: 
* Device Usage: Trump became active on Twitter in 2016, mostly using Android. From 2015-2017, Android usage decreased, while iPhone usage increased, becoming the sole device from mid-2017 to 2019.
* Behavior Across Devices: Android is more commonly used until 10AM, then iPhone is predominante until around 8PM. Over the time period of the entire dataset from Jan 2016-Jan 2019, Twitter on iPhone had the highest usage.
* Device in 2017: In March 2017, Trump switched from an Android to an iPhone. During his presidential campaign, it was theorized that Donald Trump's tweets from Android devices were written by him personally, and the tweets from iPhones were from his staff. We confirm this and we see Android tweets happened earlier in the day and we know this is when Trump tends to tweet. iPhone tweets happen later when staff would be at work and more likely to tweet. 

Sentiment Analysis:
* Plotting the sentiments for all tweets, the mean and median fall close to 0.
* Election & Inagauration Dates: We see that around the time of his election, the polarity of Trump's tweets was a significantly higher than during the time of his inaugaration. About a month after his inaugaration, there was a sharp increase in his tweet polarity, and it increased steadily until January 2018, when it took another dip.
* Election and Inaugaration Dates Mentions of "Fake News": Usage of the term "fake news" significantly increases between election and inaugaration, and has spiked up and down ever since. This may be correlated with any news release events that upset him, so he asserts these articles are false and "fake news".
* Distributions of Sentiments for tweets containing certain keywords: I create overlaid plots of sentiment distribution for tweets containing 2 keywords.
  * Trump has more positive Tweets about Fox than the New York Times. 
  * There seem to be more positive tweets about drugs than god, and more positive tweets for drugs than fod food - a funny phenomenon.
  * Mentions of 'immigrant' have lower polarity than mentions of 'border'.
  * Mentions of 'mexico' have lower polarity than mentions of 'military'.
  * Mentions of 'usa' have more positive tweets than mentions of 'russia'.
* Sentiments for Tweets with vs without hashtags/links: Tweets with hashtag or links have more neutral polarity, the mode is higher and centered around 0, the distribution is unimodal. For no hashtag or link, there is much more spread, and it is bimodal.

Engagement: The top 20 most retweeted words include 'illegally', 'human', 'christmas', 'mccabe', 'kavanaugh', 'mainstream', and 'immigrants'. 

For more details ressults, please see [Trump-Twitter-Text.ipynb](https://github.com/emeri-z/twitter-sentiment-analysis/blob/master/Trump-Twitter-Text.ipynb)

### Future work:


1. I have scraped Tweets with tweepy and Twitter’s API before, and I have included code in “twitter_scrape.ipynb”. I hope to repeat this analysis on more recent tweets, particularly as rumors and memes of WWIII circulate the internet. 
2. This is a really amazing interactive article by the NYTimes. In the future, I hope to be able to create something of the sort: https://www.nytimes.com/interactive/2019/11/02/us/politics/trump-twitter-presidency.html
3. I could dive deeper into the history of Trump’s presidencies, aligning real-word events and media releases with the sentiment of his Tweets.
4. For a more ML geared approach, I can extend this by building a Naive Bayes Classifier.

I am always open to feedback; feel free to ping me @emeri.zhang@berkeley.edu! I will push as I make updates to this project.
