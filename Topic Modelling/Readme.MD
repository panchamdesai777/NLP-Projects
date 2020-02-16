# Topic Modeling of News Headlines

![Alt Text](https://bugra.github.io/static/images/work/notes/2017/2/5/blei_lda_illustration.png)

## Problem Statement
Time to put your understanding of Topic Modelling into practice! You have a dataset of news headlines sourced from the reputable Australian news source ABC (Australian Broadcasting Corp.) over a period of 15 years.<br/> 
If you dig into the keywords, you will see all the important episodes shaping the last decade and how they evolved over time. <br/> 
Ex: financial crisis, iraq war, multiple US elections, ecological disasters, terrorism, famous people, Australian crimes etc. <br/> 
A much better way to comprehend these topics would be using topic modelling to find out relevant topics within a particular time frame.<br/> 
The main goal of this problem is to leverage the power of techniques like LSA (Latent Semantic Analysis) and LDA (Latent Dirichlet Allocation) to assign topics to unseen news headlines.<br/> 

## Approach to solve this problem
* Load and preprocess data<br/> 
In this task you will be loading and preprocessing data. Preprocessing involves retaining only alphabets in the headlines.<br/> 

* Which is the most frequently occurring word in the document?
In order to get an idea of the topics, the most frequently occuring word in the entire corpus would be of great help.<br/> 
These frequently occuring words have a high probability of occuring in the topics and so lets visualize them. <br/> 

* Topic Modelling with LSA
In the previous tasks you preprocessed data and also had a glimpse into possible words in your topics. Now use LSA (Latent Semantic Analysis) to assign topics to every headline. <br/> 
Since almost every word has some chance of getting assigned to a particular topic,you will be choosing only the 10 most important words for every topic<br/> 

* Topic Modelling with LDA
Use the gensim package to perform topic modelling with LDA (Latent Dirichlet Allocation) this time. <br/> 
A function clean_doc has been provided for you which removes stopwords and punctuation marks and also lemmatizes every word in headline.<br/> 

* Coherence score to determine the optimum number of topics
Are 5 topics sufficient for summarizing all the given news headlines?
Observe it by harnessing the power of coherence scores to determine what should be the number of topics for the data

## Why solve it
Solving it will help you apply the following skills:<br/> 
* Text preprocessing techniques like tokenization, stopword removal, POS tagging etc.
* Enhance your data visualization skills
* Topic modelling with LSA (Latent Semantic Analysis) and LDA (Latent Dirichlet Allocation)
* Use coherence score to determine the optimum number of topics
