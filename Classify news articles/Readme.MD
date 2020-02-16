# Classify The News Articles

![Alt txt](https://www.blumeglobal.com/wp-content/uploads/2018/11/NLP-image.jpg)

## Problem Statement
You are given references to news pages collected from an web aggregator in the period from 10-March-2014 to 10-August-2014. <br/>
The resources are grouped into categories that represent pages discussing the same story. <br/>
News categories included in this dataset include business(b); science and technology(t); entertainment(e); and health(h).<br/>
The goal is to predict which class a particular resource belongs to given the title of the resource.<br/>

## About the dataset
This dataset comes from the UCI Machine Learning Repository. In total there are 422937 resources available in the dataset. <br/>
The columns included in this dataset are:<br/>
* ID: the numeric ID of the article
* TITLE: the headline of the article
* URL: the URL of the article
* PUBLISHER: the publisher of the article
* CATEGORY: the category of the news item; one of: b:business, t:science and technology, e: entertainment and m:health
* STORY: alphanumeric ID of the news story that the article discusses
* HOSTNAME: hostname where the article was posted
* IMESTAMP: approximate timestamp of the article's publication, given in Unix time (seconds since midnight on Jan 1, 1970)

## Approach to Solve the problem <br/>
* Load data and observe class distributions
First task for you guys is to load data, take only the relevant columns and observing the distribution of the class labels.<br/>
* Preprocess data and split into training and test sets <br/>
In the previous task you selected the required subset of data and observed the distribution of labels.  <br/>
Now time to preprocess text data by doing the following steps on the TITLE column -  <br/>
Retaining only alphabets (Using regular expressions) <br/>
Removing stopwords (Using nltk library) <br/>
Splitting into train and test sets (Uisng scikit-learn library) <br/>
* Vectorize with Bag-of-words and TF-IDF approach
After cleaning data its time to vectorize data so that it can be fed into an ML algorithm. <br/>
You will be doing it with two approaches: Bag-of-words and TF-IDF. <br/>
* Predicting with Multinomial Naive Bayes <br/>
Multinomial Naive Bayes is an algorithm that can be used for the purpose of multi-class classification.<br/>
You will be using it to train and test it on both the versions i.e. <br/>
Bag-of-words and TF-IDF ones and then checking the accuracy on both of them <br/>
* Predicting with Logistic Regression
Logistic Regression can be used for binary classification but when combined with OneVsRest classifer, <br/>
it can perform multiclass classification as well. <br/>
You will be using one such algorithm to train and test it on both the versions i.e. <br/>
Bag-of-words and TF-IDF ones and then checking the accuracy on both of them <br/>

## Why solve it ?
Solving it will reinforce the following concepts of text analytics:<br/>

* Preprocess text data with tokenization, stopword removal etc
* Vectorize data using Bag-of-words and TF-IDF approaches
* Apply classifiers (Logistic and Multinomial Naive Bayes) to perform multi-class classification



