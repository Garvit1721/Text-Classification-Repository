# Text Classification using Naive Bayes and Support Vector Machine (SVM)

## Description

This repository contains Python scripts for performing text classification on movie review data using Naive Bayes and Support Vector Machine (SVM) classifiers. The dataset consists of movie reviews categorized as positive or negative sentiments, which are used to train and evaluate the classifiers.

## Data Loading and Preprocessing

The scripts load the movie review dataset from NLTK's movie_reviews corpus and preprocess the text data by tokenizing, lemmatizing, and removing stopwords and punctuation. The cleaned text data is then converted into numerical features using a bag-of-words approach.

## Model Training and Evaluation

Two classifiers, Naive Bayes and SVM, are trained on the numerical features extracted from the text data. The models are trained using the training data and evaluated on the testing data to measure their accuracy.

## Feature Extraction

The most common words are extracted from the training data and used as features for the classifiers. These features are represented as a feature dictionary, indicating whether each word is present in a given document.

## Model Comparison

The accuracy of the Naive Bayes and SVM classifiers is compared using the nltk.classify.accuracy function. Additionally, the most informative features are displayed for the Naive Bayes classifier.

## Sklearn Integration

The NLTK classifiers are integrated with scikit-learn using the SklearnClassifier wrapper. The classifiers are trained and evaluated using the same training and testing data to compare their performance with the NLTK classifiers.

## Feature Engineering with Sklearn

Sklearn's CountVectorizer is used to convert the text data into numerical features. The most common n-grams (2-grams and 3-grams) are extracted as features, and the dataset is transformed into a matrix of token counts.

## Model Training with Sklearn

The SVM classifier is trained using the transformed training data, and its performance is evaluated on the transformed testing data to measure its accuracy.
