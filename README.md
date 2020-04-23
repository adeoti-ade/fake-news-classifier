# fake-news-classifier
This is capstone project required by Udacity to pass the Data Science NanoDegree. The project is a classifier that aims to classify an article as either fake or real based on the title of the article and the article content. The project follows the data CRISP-DM method


### Table of Content8

1. [Background](#background)
3. [Installation](#installation)
4. [Library Used](#library)
5. [Problem Statement](#statement)
6. [Problem Questions](#questions)
6. [File Descriptions](#files)
7. [Conclusion](#conclusion)
5. [References](#reference)

## Background <a name="background"></a>

This project is a requirement of the Udacity Data Scientist Nanodegree. The purpose of the project is to provide insights into the boston housing dataset and make inference where necessary. 

## Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python.  The code should run with no issues using Python versions 3.*.

## Library Used <a name="library"></a>

The library used includes pandas for data structure and reading data into notebook, numpy for mathematical analysis, seaborn and matplotlib for data visualization and scikitlearn for model estimation

## Problem Statement <a name="statement"></a>
The genuineness of Information has become a long term issue influencing organizations and society, both for printed and computerized media. On interpersonal organizations, the compass and impacts of data spread happen at such a quick pace thus enhanced that mutilated, off base or bogus data procures an enormous potential to cause genuine effects, in practically no time, for many clients.

To provide a solution to this problem, Machine Learning comes in handy. With an historical data that contains information on fake and real news, Machine Learning can be used to classify articles as either fake or not using underlying patterns from the historical data

## Problem Questions <a name="questions"></a>

1. How fake news is distributed between yes or no?
2. What is the relationship of the word counts and upper case count in the news content?
3. what is the relationship of the word counts and stopword count in the text content?
4. what is the relationship of the word counts and stopword count in the text content
5. What is the correlation of punctuation counts and title case count in the text content
6. What is the relationship of the numeric features
The files used in this project is the boston housing data and can be downloaded [here](https://www.kaggle.com/c/fake-news/data). 


## File Descriptions <a name="files"></a>

### train.csv: A full training dataset with the following attributes
id: unique id for a news article
title: the title of a news article
author: author of the news article
text: the text of the article; could be incomplete
label: a label that marks the article as potentially unreliable 1: unreliable 0: reliable
### test.csv: A testing training dataset with all the same attributes at train.csv without the label.


## Conclusion<a name="conclusion"></a>

This notebook uses machine learning process to classify fake news. To provide the best model, the researcher made of three set of features to train the model. The model was trained on the NLP pipeline of article title, NLP pipeline of the article content and a set of manual features extracted from the article title and content. 

### Reflection

This project revealed that in order to classify fake news, both the article title and text are good features as they both gave a good precision and recall score. Furthermore, the project also revealed that text features like, number of some part of speech, punctuation counts, word counts, etc. also are good features in classifying fake news. The project however showed that Support Vector Classifier seems to be the best classifier among the classifiers used in this project

### Improvement

This project was created without any hyperparameter tuning. In order to improve the model, one may perform some slight parameter tuning. Also, one may create a pipeline using FeatureUnion to combine the three(3) features and create a single model.

## References <a name="reference"></a>

[Predicting the Survival of Titanic Passengers](https://towardsdatascience.com/predicting-the-survival-of-titanic-passengers-30870ccc7e8)

[Tips for Effective Data Visualization](https://towardsdatascience.com/tips-for-effective-data-visualization-d4b2af91db37)
