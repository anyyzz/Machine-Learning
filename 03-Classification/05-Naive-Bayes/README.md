# Naive Bayes

## Overview

Naive Bayes is a supervised machine learning algorithm used for classification. It uses probability to estimate how likely an observation is to belong to each class and assigns it to the class with the highest probability.

Unlike distance-based or boundary-based classifiers such as K-NN and SVM, Naive Bayes makes predictions by comparing the probabilities of each possible class.

In this notebook, I used Gaussian Naive Bayes to predict whether a user will purchase an SUV based on their age and estimated salary. The "naive" assumption is that the features are conditionally independent given the class. In reality, Age and Estimated Salary may be correlated, since salary can generally increase with age, but Naive Bayes assumes independence to simplify the probability calculations.

Gaussian Naive Bayes also assumes that the continuous features follow a Gaussian (normal) distribution within each class.

## Dataset

This implementation uses the Social_Network_Ads dataset.

- **Independent Variables (X):** Age, Estimated Salary
- **Dependent Variable (y):** Purchased (0 = No, 1 = Yes)

## What You'll Find Here

- Splitting the dataset into training and testing sets
- Applying feature scaling to the independent variables
- Training a Gaussian Naive Bayes classifier
- Predicting whether a new user will purchase an SUV
- Evaluating the model using a confusion matrix and accuracy score
- Visualising the decision boundary on the training and test sets

## Results

The Naive Bayes model achieved an accuracy of **90%** on the test set.

For comparison, the previous models achieved:

- **Logistic Regression:** 89%
- **K-NN:** 93%
- **SVM (Linear):** 90%
- **Kernel SVM (RBF):** 93%
- **Naive Bayes:** 90%

On this dataset and test split, K-NN and Kernel SVM achieved the highest accuracy, followed by SVM (Linear) and Naive Bayes, with Logistic Regression achieving the lowest accuracy.
