# Credit_Risk_Analysis

## Overview
In this project the team applied machine learning to solve a credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we employed different techniques to train and evaluate models with unbalanced classes. We used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we oversampled the data using the RandomOverSampler and SMOTE algorithms, and undersampled the data using the ClusterCentroids algorithm. Then, we used a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. After we compared two new machine learning models that reduced bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results
### Naive Random Oversampling
- Balance accuracy score was 0.6438627638488825
- Precesion score was 0.01 high risk, 1 low risk, 0.99 average/total
- Recall score was 0.69 high risk, 0.59 low risk, 0.6 average/total

### SMOTE Oversampling
- Balance accuracy score was 0.6628910844779521
- Precesion score was 0.01 high risk, 1 low risk, 0.99 average/total
- Recall score was 0.63 high risk, 0.69 low risk, 0.60 average/total

### Undersampling
- Balance accuracy score was 0.5442661782548694
- Precesion score was 0.01 high risk, 1 low risk, 0.99 average/total
- Recall score was 0.69 high risk, 0.40 low risk, 0.4 average/total

### Combination (Over and Under) Sampling
- Balance accuracy score was 0.6386694328927748
- Precesion score was 0.01 high risk, 1 low risk, 0.99 average/total
- Recall score was 0.70 high risk, 0.57 low risk, 0.58 average/total

### Balanced Random Forest Classifier
- Balance accuracy score was 0.7887512850910909
- Precesion score was 0.01 high risk, 0 low risk, 0 average/total
- Recall score was 1 high risk, 0 low risk, 0.01 average/total

### Easy Ensemble AdaBoost Classifier
- Balance accuracy score was 0.931601605553446
- Precesion score was 0.09 high risk, 1 low risk, 0.99 average/total
- Recall score was 0.92 high risk, 0.94 low risk, 0.94 average/total

## Summary
From our results, the machine learning models that performed the best was the Easy Ensemble AdaBoost classifier with a balance accuracy score of 0.93. None of the other classifiers came even close as most of them performed around 0.6. We would recommend the Easy Ensemble model based on its performance. 
