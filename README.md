# Iris Classification with PCA and Distance-Based Classifiers: Python Implementation

This repository contains a project that uses the Iris dataset to perform classification using multiple classifiers along with dimensionality reduction via PCA (Principal Component Analysis). Various distance-based classification algorithms were applied and evaluated through cross-validation and confusion matrices.

## Contents

- `bezdekIris.data`: Iris dataset used for training and testing.
- `QDA, Minimum distance, Mahalanobis, PCA_iris.py`: Main code implementing the classifiers and PCA.

## Project Description

This project addresses the classification problem of the Iris dataset using dimensionality reduction techniques and distance-based classifiers. The implemented classifiers were:

1. **Minimum Distance Classifier**
2. **Mahalanobis Distance Classifier**
3. **Quadratic Discriminant Analysis (QDA)**

### Dimensionality Reduction with PCA

Principal Component Analysis (PCA) was applied to reduce the feature space to two principal components, which facilitates visualization and improves classifier performance.

### Cross-Validation and Test Accuracy

Cross-validation techniques were used to evaluate the performance of the classifiers in terms of training and testing accuracy.

## Implemented Classifiers

### 1. **Minimum Distance Classifier**
A minimum distance classifier was implemented using Euclidean distance. The classifier's performance was evaluated using cross-validation, and the results were presented in a confusion matrix.

- **Accuracy (Training - Cross Validation):** `0.858`
- **Accuracy (Test):** `0.933`

### 2. **Mahalanobis Distance Classifier**
A Mahalanobis distance-based classifier was applied to improve accuracy by considering correlations between features.

- **Accuracy (Training - Cross Validation):** `0.916`
- **Accuracy (Test):** `0.366`

### 3. **Quadratic Discriminant Analysis (QDA)**
Finally, Quadratic Discriminant Analysis (QDA) was implemented, allowing classification by considering different shapes of class distributions.

- **Accuracy (Training - Cross Validation):** `0.916`
- **Accuracy (Test):** `0.900`

## Results

Three confusion matrices were generated for each of the classifiers mentioned above. These results show the ability of the models to distinguish between the three Iris species based on the provided features:

1. **Minimum Distance with PCA Confusion Matrix**
2. **Mahalanobis Distance with PCA Confusion Matrix**
3. **QDA with PCA Confusion Matrix**

## Requirements

To run this project, ensure you have the following Python packages installed:

- `numpy`
- `pandas`
- `scikit-learn`
- `matplotlib`
- `seaborn`

## Conclusion

This project demonstrates the effectiveness of various distance-based classifiers on the Iris dataset, improving feature interpretation using PCA. While the Minimum Distance Classifier and QDA provided high levels of classification accuracy, the Mahalanobis Classifier showed lower performance compared to the other two.
