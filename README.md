Twitter Sentiment Analysis

Overview

This project aims to perform sentiment analysis on a large dataset of tweets to classify them as positive or negative. Sentiment analysis is a natural language processing (NLP) technique used to determine whether a piece of text is positive, negative, or neutral. In this project, the focus is on building and comparing several machine learning models to accurately classify the sentiments expressed in tweets.

Dataset

The dataset used in this project consists of 1.6 million tweets, each labeled as either positive or negative. The dataset includes the following columns:

target: Sentiment label (0 for negative, 1 for positive)
id: Unique identifier for each tweet
date: Date and time when the tweet was created
flag: Query flag (unused in this project)
user: Username of the tweet author
text: The content of the tweet

The project requires the following Python libraries:

numpy
pandas
re
nltk
scikit-learn
pickle

Preprocessing

Data Cleaning: Remove URLs, usernames, and non-alphabetic characters from the tweets.
Stemming: Reduce words to their root form using the Porter Stemmer.
Stopwords Removal: Remove common English stopwords to reduce noise.

Feature Extraction

We use the TF-IDF vectorizer to convert the cleaned text data into numerical features suitable for machine learning models.

Models

We train and compare the following machine learning models: Logistic Regression and Random Forest

The models are evaluated based on their accuracy on the training and test datasets. Training and prediction times are also measured to compare the performance of each model.

Results

The results of the model evaluations, including accuracy scores and training times, are detailed in the notebooks/model_comparison.ipynb notebook.

Future Work

Implement additional preprocessing techniques such as lemmatization.
Including emojis for sentiment analysis

Acknowledgements

The dataset used in this project is provided by Kaggle and is publicly available here['https://www.kaggle.com/datasets/kazanova/sentiment140'].