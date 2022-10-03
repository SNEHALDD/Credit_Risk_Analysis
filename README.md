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


## Results: 

1) Deliverable 1: Use Resampling Models to Predict Credit Risk
--- Oversampling using Naive Random Sampling
- An accuracy score for the model
- A confusion matrix has been generated 
- An imbalanced classification report
<img width="760" alt="Naive Random Oversampling" src="https://user-images.githubusercontent.com/106944351/193426221-d5d40804-aab5-4514-b7d4-ef0cca2b1463.png">

Accuracy Score: 64.5%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 61%
Recall Low Risk: 68%

--- Oversampling using SMOTE Oversampling
- An accuracy score for the model
- A confusion matrix has been generated 
- An imbalanced classification report
<img width="751" alt="SMOTE Oversampling" src="https://user-images.githubusercontent.com/106944351/193426234-1b6a8588-b168-4a29-b56e-4cd1f0c81a6a.png">

Accuracy Score: 62.3%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 61%
Recall Low Risk: 64%

If we compare naive random oversampling algorithm and the SMOTE algorithm, both gives almost similar results. Naive Random Oversampling gives better accuracy which is 64.5%.

--- Undersampling using Cluster Centroid Algorithm
- An accuracy score for the model
- A confusion matrix has been generated 
- An imbalanced classification report
<img width="758" alt="Undersampling using Cluster Centroid Algorithm" src="https://user-images.githubusercontent.com/106944351/193426254-5426b6de-a9f4-4d49-a6ab-e9685bfae995.png">

Accuracy Score: 62.3%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 61%
Recall Low Risk: 57%

If we compare Cluster Centroid Algorithm with naive random oversampling algorithm and the SMOTE algorithm, again Naive Random Oversampling gives better accuracy which is 64.5%.

2) Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
Use the SMOTEENN algorithm to Predict Credit Risk
Combination Over and under sampling algorithm
- An accuracy score for the model
- A confusion matrix
- An imbalanced classification report
<img width="740" alt="SMOTEEN - Over and under sampling algorithm" src="https://user-images.githubusercontent.com/106944351/193426269-2a160e2a-4657-4cf2-8c36-a41e154f10b6.png">

Accuracy Score: 59%
Precision High Risk: 1%
Precision Low Risk: 100%
Recall High Risk: 70%
Recall Low Risk: 58%

If we compare SMOTEENN algorithm with Cluster Centroid Algorithm, naive random oversampling algorithm and the SMOTE algorithm, again Naive Random Oversampling gives better accuracy which is 64.5% which is higher that all.

3) Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
The BalancedRandomForestClassifier algorithm:
- An accuracy score for the model
<img width="599" alt="BalancedRandomForestClassifier- accuracy score" src="https://user-images.githubusercontent.com/106944351/193426291-a9380732-c54a-4cd0-8dc0-7cb87d1d8c1d.png">

- A confusion matrix
<img width="1073" alt="BalancedRandomForestClassifier- confusion matrix" src="https://user-images.githubusercontent.com/106944351/193426300-2f5d3a64-106a-4b6d-a8eb-19e6709292ec.png">

- An imbalanced classification report
<img width="863" alt="BalancedRandomForestClassifier- classificatio report" src="https://user-images.githubusercontent.com/106944351/193426314-3198ed80-89a9-457b-822c-2217e648a0c0.png">

- The features are sorted in descending order by feature importance
<img width="696" alt="BalancedRandomForestClassifier-features" src="https://user-images.githubusercontent.com/106944351/193426323-496155fa-fca1-4df3-b435-3841a4b1c6ec.png">

Accuracy Score: 66%
Precision High Risk: 72%
Precision Low Risk: 100%
Recall High Risk: 32%
Recall Low Risk: 100%


The EasyEnsembleClassifier algorithm
- An accuracy score of the model & confusion matrix
<img width="1059" alt="EasyEnsembleClassifier-accuracy and confusion" src="https://user-images.githubusercontent.com/106944351/193426340-3de55d04-ade1-4e60-9137-13dd5abfa896.png">

- An imbalanced classification report 
<img width="791" alt="EasyEnsembleClassifier" src="https://user-images.githubusercontent.com/106944351/193426352-750abd9a-0b1f-4c8f-ac50-a44cb5b0a45f.png">

Accuracy Score: 92%
Precision High Risk: 7%
Precision Low Risk: 100%
Recall High Risk: 91%
Recall Low Risk: 100%

If we compare Balanced Random Forest Classifier and an Easy Ensemble AdaBoost classifier, EasyEnsembleClassifier algorithm performs best. it gives accuracy of 92%. 

## Summary: Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. If you do not recommend any of the models, justify your reasoning.
After considering the balanced accuracy score of all the models, Easy Ensemble AdaBoost classifier proves to be the best machine learning model with this dataset since it is giving us the best accuracy among all which is 92%. I would suggest that Easy Ensemble AdaBoost classifier can be the best machine learning model.
