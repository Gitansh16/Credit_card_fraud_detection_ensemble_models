# Credit Card Fraud Detection using Ensemble Models

## Project Overview

This project focuses on detecting credit card fraud using machine learning models. The goal is to identify fraudulent transactions from a highly imbalanced dataset, comparing the performance of individual models with ensemble techniques. We utilize several classifiers and combine them using ensemble methods to enhance the accuracy and robustness of the predictions.

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset](#dataset)
- [Problem Statement](#problem-statement)
- [Models Implemented](#models-implemented)
- [Ensemble Techniques](#ensemble-techniques)
- [Performance Evaluation](#performance-evaluation)
- [Usage](#usage)


## Dataset

The dataset used for this project is the **[Credit Card Fraud Detection Dataset](https://www.kaggle.com/mlg-ulb/creditcardfraud)**. It contains transactions made by European cardholders over two days in September 2013. Out of 284,807 transactions, 492 are fraudulent, representing a highly imbalanced dataset.

### Key Features:
- **Number of Instances**: 284,807
- **Fraudulent Transactions**: 492
- **Features**: 30 anonymized features (`V1` to `V28`), along with `Time`, `Amount`, and the `Class` label (fraudulent or not).

## Problem Statement

Credit card fraud is a significant issue faced by financial institutions and cardholders. Detecting fraud accurately while minimizing false positives is crucial. Due to the imbalance in the dataset, traditional machine learning models tend to underperform. To address this, we build ensemble models by comparing the performance of various classifiers and combining them to improve fraud detection accuracy.

## Models Implemented

We compare the following machine learning models:

- **Logistic Regression**
- **Random Forest**
- **Support Vector Machines (SVM)**
- **Gradient Boosting Machines (XGBoost)**

## Ensemble Techniques

After evaluating the performance of individual models, we applied ensemble methods to boost the detection capability. The following ensemble techniques were used:

- **Voting Classifier**: Combines predictions from multiple models (soft and hard voting).
- **Stacking**: Combined several models as base learners and used a meta-model for final predictions.

## Performance Evaluation

The performance of the models is evaluated using the following metrics:

- **Accuracy**: Overall accuracy on the test set.
- **Precision**: The proportion of true positives over all predicted positives.
- **Recall**: The ability of the model to detect all actual fraud cases.
- **F1 Score**: Harmonic mean of precision and recall, providing a balanced measure.
- **AUC-ROC**: Area Under the Receiver Operating Characteristic Curve, which evaluates the trade-off between true positives and false positives.

The ensemble models showed significant improvements over individual models, particularly in terms of precision and recall, which are crucial for fraud detection in an imbalanced dataset.

## Usage

1. Clone the repository:

```bash
git clone https://github.com/your-username/credit-card-fraud-detection.git
cd credit-card-fraud-detection


