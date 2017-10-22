# Aibrite NLP Sandbox
An NLP sandbox, utilizing live tweets and labeling the tweets positive and negative.
The training data set is nltk's built-in review data set.
Application also includes a plotter that displays the live positive/negative line of the tweets.

# About the App
The application utilizes `nltk`'s built-in tools and data sets to train a model, in order to detect positive and negative quotes.
The app simultaneously utilizes:
1. Multinomial Naive Bayes Classifier
2. Bernoulli Naive Bayes Classifier
3. Logistic Regression Naive Bayes Classifier
4. SGD Naive Bayes Classifier
5. Linear SVC Naive Bayes Classifier
6. NuSVC Naive Bayes Classifier

Also, a `Voted_Classifier` is included, that implements voting to all of the above classifiers and returns the highest voted label.

# How to Run
1. Replace the consumer key and the secret key in `twitter/twitterbase.py` with your keys.
2. Change the subject at `line 29` of `run_tweet_analyzer.py`
3. If you are running the app for the first time, leave the `first_run=True` at `line 18` of `run_tweet_analyzer.py` as `True`. Else, set it to `False`
3. Execute `setandrun.sh` and you are ready to go.