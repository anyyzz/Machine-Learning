# Support Vector Machine (SVM)

## Overview

Support Vector Machine (SVM) is a supervised machine learning algorithm used for classification. It finds a decision boundary that separates different classes while maximising the margin between the boundary and the closest observations. These closest observations are known as support vectors and help determine the position of the boundary.

In this notebook, I trained an SVM classifier using Scikit-learn to predict whether a user will purchase an SUV based on their age and estimated salary. A linear kernel was used, meaning the model learns a linear decision boundary between the two classes.

Feature scaling is applied to the independent variables before training so that Age and Estimated Salary are on comparable scales when determining the decision boundary.

## Dataset

This implementation uses the Social_Network_Ads dataset.

- **Independent Variables (X):** Age, Estimated Salary
- **Dependent Variable (y):** Purchased (0 = No, 1 = Yes)

## What You'll Find Here

- Splitting the dataset into training and testing sets
- Applying feature scaling to the independent variables
- Training an SVM classifier using a linear kernel
- Predicting whether a new user will purchase an SUV
- Evaluating the model using a confusion matrix and accuracy score
- Visualising the decision boundary on the training and test sets

## Results

The SVM model achieved an accuracy of **90%** on the test set.

For comparison, the previous models achieved:

- **Logistic Regression:** 89%
- **K-NN:** 93%
- **SVM (Linear):** 90%

On this dataset and test split, K-NN achieved the highest accuracy, followed by SVM and Logistic Regression.
