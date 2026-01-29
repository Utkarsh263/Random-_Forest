# Credit Card Fraud Detection – Model Description

## Problem Statement
The objective of this task is to identify fraudulent credit card transactions from a highly imbalanced dataset. Since fraudulent cases are rare, the model must prioritize correctly identifying fraud while minimizing false negatives.

## Baseline Model Used
Logistic Regression is used as an initial baseline model to establish a performance reference. It is a linear classifier that requires feature scaling and performs reasonably on simple patterns, but its effectiveness is limited when dealing with severe class imbalance and complex, non-linear relationships.

## Final Model Applied
Random Forest Classifier is used as the primary model to solve the fraud detection problem. It is an ensemble learning technique that combines multiple decision trees to improve predictive performance. The model captures non-linear patterns in the data and is more robust to class imbalance.

## Model Configuration
- Number of trees (`n_estimators`): 100  
- Class weighting: Balanced to address data imbalance  
- Random state: Fixed for reproducibility  

## Reason for Model Selection
Random Forest is selected as the final model because it provides better fraud detection performance compared to the baseline model, particularly in terms of recall and F1-score. This makes it more suitable for identifying rare fraudulent transactions in real-world scenarios.
