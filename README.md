# Sentiment Analysis for the IMDb Movie Reviews dataset

## Introduction
This exercise was completed in preparation for the Natural Language Processing (NLP) course at [Tehran University](https://ut.ac.ir/en) in April 2020.

In this exercise, I implemented a simple Naïve Bayes classifier for sentiment classification. For this purpose, I used the film review corpus. NLTK has provided copies of this dataset. This dataset has categorized each review into two categories, positive or negative. You can use the following command to use this data set:
```
import nltk
nltk.download('movie_reviews')
```

### Exercise steps
* __Preprocess__: I performed the necessary pre-processing on the data including the removal of Stop Words, Tokenization, Normalization, Punctuation removing, and ...

* __Feature Extraction__: In order to be able to train a classifier, it is necessary to extract some features from the text.
I extracted features in four different ways :
    * Using top n frequent words
    * Using Bag of Words of unigrams
    * Using Bag of Words of bigrams
    * Using Bag of Words of ngrams

* __Classifier Training__: In this step, using the features extracted in the previous step, the Naïve Bayes classifier was trained. I used the k-fold validation method on the training data and considered k as 5.

* __Model Evaluation__: At this point, I evaluated the classifier I had trained. To evaluate I reported Precision, Recall, Accuracy, and F1 scores.


[Using top n frequent words - notebook](CA2-TopN.ipynb) <br>
[Using Bag of unigrams - notebook](CA2-BOW-Unigram.ipynb) <br>
[Using Bag of bigrams - notebook](CA2-BOW-Bigram.ipynb) <br>
[Using Bag of ngrams - notebook](CA2-BOW-Ngram.ipynb) <br>
