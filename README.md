# Credit_Risk_Analysis

## Overview of the analysis: 
We will apply machine learning to solve a real-world challenge. Our primary focus will be credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. We employed different techniques to train and evaluate models with unbalanced classes. We used imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. We took the credit card credit dataset from LendingClub, a peer-to-peer lending services company, and oversampled the data using the RandomOverSampler and SMOTE algorithms. And undersampled the data using the ClusterCentroids algorithm. We then used combinatorial approach of over- and undersampling using the SMOTEENN algorithm. We then compared two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. And lastly, we evaluated the performance of these models and made a written recommendation on whether they should be used to predict credit risk.

## Results:
The results for the six machine learning models including their respective balanced accuracy, precision, and recall scores are as follows:      

### Naive Random Oversampling
![1-Naive Random Oversampling](https://github.com/ScottyMacCVC/Credit_Risk_Analysis/blob/main/Images/1-Naive%20Random%20Oversampling.PNG)     
1. Balanced Accuracy: 0.6612700484668286
2. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
3. Recall: High/Low risk = .66/.67

### SMOTE Oversampling
![2-SMOTE Oversampling](https://github.com/ScottyMacCVC/Credit_Risk_Analysis/blob/main/Images/2-SMOTE%20Oversampling.PNG)     
1. Balanced Accuracy: 0.6303296388959394
2. Precision: The precision is low for High-risk loans and is high for Low-risk loans.
3. Recall: High/Low risk = .62/.64

### Undersampling
![3-Undersampling](https://github.com/ScottyMacCVC/Credit_Risk_Analysis/blob/main/Images/3-Undersampling.PNG)     
1. Balanced Accuracy: 0.6303296388959394
2. Precision: Precision is low for high-risk loans and high for Low-risk loans.
3. Recall: High/Low risk = .63/.40

### Combination Under-Over Sampling
![4-Combination Under-Over Sampling](https://github.com/ScottyMacCVC/Credit_Risk_Analysis/blob/main/Images/4-Combination%20Under-Over%20Sampling.PNG)     
1. Balanced Accuracy: 0.5173713090878325
2. Precision: Precision is low for High-risk loans and high for Low-risk loans.
3. Recall: High/Low risk = .70/.57

### Balanced Random Forest Classifier
![5-Balanced Random Forest Classifier.](https://github.com/ScottyMacCVC/Credit_Risk_Analysis/blob/main/Images/5-Balanced%20Random%20Forest%20Classifier.PNG)     
1. Balanced Accuracy: 0.7877672625306695
2. Precision: Precision is low for high-risk loans and high for Low-risk loans.
3. Recall: High/Low risk = .67/.91

### Easy Ensemble AdaBoost Classifier
![6-Easy Ensemble AdaBoost Classifier](https://github.com/ScottyMacCVC/Credit_Risk_Analysis/blob/main/Images/6-Easy%20Ensemble%20AdaBoost%20Classifier.PNG)     
1. Balanced Accuracy: 0.925427358175101
2. Precision: Precision is low for high-risk loans and high for Low-risk loans.
3. Recall: High/Low risk = .91/.94


## Summary: 
Our target goal is 1. The compared accuracies were measured between 0 and 1. The closeer to 1, the better the score. The Easy Ensenble AdaBoost Classifier is the stronges model with .93 accuracy. The other data models were at least 10% less accurate. The precision fell within a similar range of each other. Based on these notes, we would want to use the Easy Ensemble AdaBoost Classifier as the most opportune machine learning model to further our credit card analysis. 
