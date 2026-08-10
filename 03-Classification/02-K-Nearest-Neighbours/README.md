# K-Nearest Neighbours (K-NN)

## Overview

K-Nearest Neighbours (K-NN) is a supervised machine learning algorithm used for classification. It is a distance-based, non-parametric algorithm that classifies a new observation based on the classes of its closest neighbours. By relying on local neighbourhoods rather than a fixed equation, K-NN can capture non-linear decision boundaries.

In this notebook, I trained a K-NN classifier using Scikit-learn to predict whether a user will purchase an SUV based on their age and estimated salary. Since K-NN relies on distances between observations, feature scaling is important so that both variables contribute fairly. The model uses 5 nearest neighbours with Minkowski distance and `p = 2`, which corresponds to Euclidean distance.

## Dataset

This implementation uses the Social_Network_Ads dataset.

- **Independent Variables (X):** Age, Estimated Salary
- **Dependent Variable (y):** Purchased (0 = No, 1 = Yes)

## What You'll Find Here

- Splitting the dataset into training and testing sets
- Applying feature scaling to the independent variables
- Training a K-NN classifier using 5 nearest neighbours, Minkowski distance, and `p = 2`
- Predicting whether a new user will purchase an SUV
- Evaluating the model using a confusion matrix and accuracy score
- Visualising the decision boundary on the training and test sets

## Results

The K-NN model achieved an accuracy of **93%** on the test set, compared to **89%** achieved by the Logistic Regression model on the same dataset and test split.
