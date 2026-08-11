# Kernel SVM

## Overview

Kernel Support Vector Machine (Kernel SVM) is a supervised machine learning algorithm used for classification. It uses a kernel function to transform the data into a higher-dimensional space, allowing SVM to find a decision boundary when the classes cannot be separated effectively by a straight line.

In this notebook, I trained a Kernel SVM classifier using Scikit-learn to predict whether a user will purchase an SUV based on their age and estimated salary. The Radial Basis Function (RBF) kernel was used to capture non-linear relationships and create a non-linear decision boundary between the classes.

Feature scaling is applied to the independent variables before training so that Age and Estimated Salary are on comparable scales when determining the decision boundary.

## Dataset

This implementation uses the Social_Network_Ads dataset.

- **Independent Variables (X):** Age, Estimated Salary
- **Dependent Variable (y):** Purchased (0 = No, 1 = Yes)

## What You'll Find Here

- Splitting the dataset into training and testing sets
- Applying feature scaling to the independent variables
- Training a Kernel SVM classifier using the RBF kernel
- Predicting whether a new user will purchase an SUV
- Evaluating the model using a confusion matrix and accuracy score
- Visualising the non-linear decision boundary on the training and test sets

## Results

The Kernel SVM model achieved an accuracy of **93%** on the test set.

For comparison, the previous models achieved:

- **Logistic Regression:** 89%
- **K-NN:** 93%
- **SVM (Linear):** 90%
- **Kernel SVM (RBF):** 93%

On this dataset and test split, K-NN and Kernel SVM achieved the highest accuracy, followed by SVM (Linear) and Logistic Regression.

The results also show how changing the SVM kernel from linear to RBF affected performance on the same dataset and test split.
