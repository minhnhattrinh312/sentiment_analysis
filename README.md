# dataset

* The Twitter dataset used to train and validate our models is a combination
of the University of Michigan Kaggle competition dataset  and the "Twitter
Sentiment corpus" created by Neik Sanders . In total, these datasets contain
1,578,627 tweets labeled as either _positive_ or _negative_.
You can get dataset [here](https://drive.google.com/open?id=1FNl79LtBEnhXx4NKoPubwThERuZC6WtP)! 

* we also use **GloVe(Global Vectors for Word Representation)** for pre-trained in our embedding layer.(you can download Glove for twitters [here](http://nlp.stanford.edu/data/glove.twitter.27B.zip) ^^

# train

1. we process data by many ways such as: 
  * URLs are replaced by the <url> token.
  * Any letter repeated more than 2 times in a
row is replaced by 2 repetitions of that letter
(for example, “sooooo” is replaced by “soo”)
  * fix wrong words by using **dicos** dataset
  * Several emoticons are replaced by the tokens
  * All tweets are lowercased.

2. we use a combination of LSTM and CNN 

# result

we get the accurary to **83,7%** which is higher **8,5%** in this [paper](https://www.academia.edu/35947062/Twitter_Sentiment_Analysis_using_combined_LSTM-CNN_Models) with the same dataset.

## note: all file in this project we run on https://colab.research.google.com 

