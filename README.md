# Tweet_Sentiment_Extraction
Extract support phrases for sentiment labels
<br>Data source: https://www.kaggle.com/c/tweet-sentiment-extraction/overview

# Project Aim:
### Create an algorithm to capture word/phrase in tweet that reflects the sentiment
To better understand emotion in tweet, a model needs to be constructed to extract word/phrase in text that defines the sentiment. For this project, sentiment for each tweet is provided and the algorithm captures the word/phrase in text that best supports the sentiment for the tweet. Three categories of sentiment are defined: **neutral**, **positive** and **negative**.

# Approach:
### Named Entity Recognition (NER) -- spaCy
### Named Entity Recognition (NER) -- BERT
### Question Answering (QA) -- BERT

# Evaluation metric:
<br>**word-level Jaccard score**
<br>https://towardsdatascience.com/overview-of-text-similarity-metrics-3397c4601f50

<br>This project has 5 sections with code and detailed explanation in 5 jupyter notebooks.

* **Part I: Exploratory data analysis**
<br>Explore wordcount and Jaccard similarity score between text and selected text (extracted text that supports the sentiment) for each tweet.
* **Part II: Named Entity Recognition (NER) -- spaCy**
<br>Build named entity recognition (NER) model using spaCy for tweet sentiment extraction. For each sentiment, a separate NER model is trained.
* **Part III: Named Entity Recognition (NER) -- BERT**
<br>Build named entity recognition (NER) model using BERT for tweet sentiment extraction. A single NER model is trained for all three different sentiments.
* **Part IV: Named Entity Recognition (NER) -- BERT (3 models)**
<br>Build named entity recognition (NER) model using BERT for tweet sentiment extraction. For each sentiment, a separate NER model is trained.
* **Part V: Question Answering (QA) -- BERT**
<br>Build question answering (QA) model using BERT for tweet sentiment extraction. A single QA model is trained for all three different sentiments.

## Part I: Exploratory data analysis
### Short overview of the dataset:
<br>Number of documents in training dataset: 27481
<br>Number of documents in testing dataset: 3534

<br>After removing documents with NA in `text` and `selected_text` field:
<br>Number of documents in training dataset: 27480
<br>Number of documents in testing dataset: 3534

* Distribution of the number of tweets for each sentiment.




