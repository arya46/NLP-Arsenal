# Sentiment Analysis

This project is about using several machine learning classifiers, including Recurrent Neural Networks, to predict the sentiments in text and then compare their results.

**Dataset Used**: The dataset we are going to use is very popular among researchers in Natural Language Processing, usually referred to as the [IMDb dataset](http://ai.stanford.edu/~amaas/data/sentiment/). It consists of movie reviews from the website [imdb.com](http://www.imdb.com/), each labeled as either '**pos**itive', if the reviewer enjoyed the film, or '**neg**ative' otherwise.

## What is sentiment analysis?
With the rise of online social media platforms like Twitter, Facebook and Reddit, and the proliferation of customer reviews on sites like Amazon and Yelp, we now have access, more than ever before, to massive text-based data sets! They can be analyzed in order to determine how large portions of the population feel about certain products, events, etc. This sort of analysis is called *sentiment analysis*.

## Results 
```
+-------------------+----------------+--------------+
|       Model       | Train Accuracy | Val Accuracy |
+-------------------+----------------+--------------+
|    Naive Bayes    |    0.82396     |   0.71832    |
| Gradient Boosting |    0.89236     |   0.84992    |
|     LSTM Model    |     0.9466     |   0.86588    |
+-------------------+----------------+--------------+
```

## Conclusions
As can be seen, a simple LSTM model outperforms our traditional ML algorithms. This can be attributed to the fact that, LSTM can capture temporal behavior, ie the order dependence in the input text sequences. Whereas, traditional ML algorithms do not take such things into account.