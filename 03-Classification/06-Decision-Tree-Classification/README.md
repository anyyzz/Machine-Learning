# Decision Tree Classification

## Overview

Decision Tree Classification is a supervised machine learning algorithm that classifies observations by repeatedly splitting the data into smaller regions based on feature values. These sequential decision rules form a tree-like structure, with each split leading towards a predicted class.

In this notebook, I trained a Decision Tree Classifier using Scikit-learn to predict whether a user will purchase an SUV based on their age and estimated salary. The `entropy` criterion was used to evaluate possible splits by measuring how mixed the classes are, allowing the tree to favour splits that produce purer groups.

The resulting decision boundary forms distinct rectangular regions, reflecting how the tree makes sequential threshold-based splits on individual features.

Although feature scaling is included in the classification preprocessing pipeline, it is not required for Decision Trees because their decisions are based on feature thresholds rather than distances or feature magnitudes.

## Dataset

This implementation uses the Social_Network_Ads dataset.

- **Independent Variables (X):** Age, Estimated Salary
- **Dependent Variable (y):** Purchased (0 = No, 1 = Yes)

## What You'll Find Here

- Splitting the dataset into training and testing sets
- Training a Decision Tree Classifier using the entropy criterion
- Predicting whether a new user will purchase an SUV
- Evaluating the model using a confusion matrix and accuracy score
- Visualising the decision boundary on the training and test sets

## Results

The Decision Tree Classifier achieved an accuracy of **91%** on the test set.

For comparison, the previous models achieved:

- **Logistic Regression:** 89%
- **K-NN:** 93%
- **SVM (Linear):** 90%
- **Kernel SVM (RBF):** 93%
- **Naive Bayes:** 90%
- **Decision Tree:** 91%

On this dataset and test split, K-NN and Kernel SVM achieved the highest accuracy, followed by Decision Tree, SVM (Linear) and Naive Bayes, with Logistic Regression achieving the lowest accuracy.
