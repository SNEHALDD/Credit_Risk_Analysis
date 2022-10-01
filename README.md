# Credit_Risk_Analysis

## Overview of the analysis: 
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans.
This project contains different techniques to train and evaluate models with unbalanced classes. It contains 
- use of "imbalanced-learn" and "scikit-learn" libraries to build and evaluate models using resampling.
- oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm.
- combinatorial approach of over- and undersampling using the SMOTEENN algorithm.
- comparison of two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
- evaluation of the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

Deliverable 1: Use Resampling Models to Predict Credit Risk
Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
Deliverable 4: A Written Report on the Credit Risk Analysis (README.md)


## Results: Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all six machine learning models. Use screenshots of your outputs to support your results.

1) Deliverable 1: Use Resampling Models to Predict Credit Risk
--- Oversampling using Naive Random Sampling
- An accuracy score for the model


- A confusion matrix has been generated 


- An imbalanced classification report

--- Oversampling using SMOTE Oversampling
- An accuracy score for the model


- A confusion matrix has been generated 


- An imbalanced classification report

--- Undersampling using Cluster Centroid Algorithm
- An accuracy score for the model


- A confusion matrix has been generated 


- An imbalanced classification report


2) Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
Use the SMOTEENN algorithm to Predict Credit Risk
Combination Over and under sampling algorithm

- An accuracy score for the model

- A confusion matrix

- An imbalanced classification report




3) Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
The BalancedRandomForestClassifier algorithm:
- An accuracy score for the model

- A confusion matrix

- An imbalanced classification report

- The features are sorted in descending order by feature importance

The EasyEnsembleClassifier algorithm
- An accuracy score of the model & confusion matrix


- An imbalanced classification report 



## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.