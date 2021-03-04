#   Detecting the presence of depressive characteristics in tweets.

## Project Overview
### Data Collection and preprocessing
[tweepy.ipynb](tweepy.ipynb-)
-Used social media data from the Twitter API .Using the Tweepy python library I was able to extract close to 2000 tweets using relevant keywords.
Used Natural Language Toolkit to preprocess and clean the tweets.

### Automatic Labelling.
[tweet_emotions.ipynb](ttweet_emotions.ipynb)
Attached labels to the tweets ranging from (1-5) where 1 signified least likely to be depressed while 5 signified most likely to be depressed.
Used 3 lexicons namely Affin,Vader and NRC to generate the scores .
Performed a weighted average of the scores to correctly classify the tweets.
From the NRC emotion lexicon, emotions which are common in a depressed individual like sadness and fear were assigned greater weights 
while emotions like Joy and Trust were penalised and assigned smaller weights.

### Training the Neural Network 
[model.ipynb](model.ipynb-)
Used Word2Vec to prepare a word embedding which was then fed to a simple LSTM network.


