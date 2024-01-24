# NLP : Text Classification - Classifying Articles Relevant to US Economy

## Overview

This project focuses on analyzing approximately 8000 news articles related to the US economy. Each article is tagged as either relevant or not relevant to the US economy. The main objective is to build a classification model to predict the relevance of economic news articles.

## Data Preprocessing

The following preprocessing steps were applied to the dataset:

1. **Remove Named Entities:**
   - Named entities were removed to eliminate specific references.

2. **Text Standardization:**
   - Convert text to lowercase.
   - Replace double quotes with a space.
   - Replace hyphens with spaces.
   - Remove punctuation and digits.

3. **Text Cleaning:**
   - Remove stopwords.
   - Apply lemmatization to transform words to their base forms.

## TF-IDF Vectorizer

The TF-IDF vectorizer is used to convert the preprocessed text data into a matrix of TF-IDF features. This matrix represents the importance of each term (word) in each document, providing a numerical representation for further analysis.

## Train-Test Split

The dataset is split into training and testing sets to evaluate the performance of the classification models.

## Classification Models

### Naive Bayes Classifier

1. **Gaussian Naive Bayes:**
   - Assumes that continuous features follow a Gaussian (normal) distribution.

2. **Multinomial Naive Bayes:**
   - Suitable for discrete data, commonly used in text classification with term frequencies.

### Logistic Regression Classifier

- Logistic regression is employed for binary classification tasks. It uses the logistic function to transform the linear combination of input features into a probability value between 0 and 1.

### Support Vector Machines (SVM)

- SVM is utilized for its effectiveness in high-dimensional spaces. It aims to find a hyperplane that maximizes the margin between classes.

### Decision Tree Classifier

- Decision trees are employed for their ability to model complex decision boundaries. The dataset is split based on features to create a tree-like structure for classification.

### Ensembling: Voting Classifier

- A Voting Classifier is implemented to combine predictions from multiple individual models. Both hard and soft voting strategies are explored.

## Conclusion

This project provides a comprehensive analysis of economic news articles, including preprocessing, vectorization, and the implementation of various classification models. The goal is to predict the relevance of articles to the US economy, leveraging a diverse set of machine learning techniques. The ensemble approach, through the Voting Classifier, enhances the overall model's predictive capabilities.
