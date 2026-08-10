# Logistic Regression

## Overview

Logistic Regression is a supervised machine learning algorithm used for classification. Instead of predicting a continuous value like regression, it predicts the probability of an observation belonging to a particular class.

In this notebook, I trained a Logistic Regression model using Scikit-learn to predict whether a user will purchase an SUV based on their age and estimated salary. As Logistic Regression uses a linear decision boundary, its performance can be influenced when the classes are not linearly separable.

Feature scaling is applied to the independent variables before training. The scaler is fitted only on the training data using `fit_transform()`, while the test data is transformed using `transform()` to avoid data leakage.

## Dataset

This implementation uses the Social_Network_Ads dataset.

- **Independent Variables (X):** Age, Estimated Salary
- **Dependent Variable (y):** Purchased (0 = No, 1 = Yes)

## What You'll Find Here

- Splitting the dataset into training and testing sets
- Applying feature scaling to the independent variables
- Training a Logistic Regression classifier
- Predicting whether a new user will purchase an SUV
- Evaluating the model using a confusion matrix and accuracy score
- Visualising the decision boundary on the training and test sets

## Results

The Logistic Regression model achieved an accuracy of **89%** on the test set. The confusion matrix provides further detail on the correct and incorrect classifications.
