# Credit Risk Analysis

## Overview of the Analysis

The imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling.  A credit card dataset from LendingClub was used to oversample and undersample data using RandomOverSampler, SMOTE, and ClusterCentroids algorithms.  SMOTEENN was used for the comination approach of over and undersampling.  Finally two machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, that reduce bias were used to predict credit risk.

## Results


### Random Oversampling

 - Accuracy is 63.7%
 - Precision is low for the predictive value for high risk credit at 1% and high for low risk credit at 100%
 - Recall is 62% for high risk and 65% for low risk 


### SMOTE Oversampling

 - Accuracy is 63%
 - Precision is low for the predictive value for high risk credit at 1% and high for low risk credit at 100%
 - Recall is 62% for high risk and 64% for low risk 


### ClusterCentroids Undersampling

 - Accuracy is 63%
 - Precision is low for the predictive value for high risk credit at 1% and high for low risk credit at 100%
 - Recall is 62% for high risk and 65% for low risk 


### SMOTEENN Over and Under Sampling

 - Accuracy is 63.8%
 - Precision is low for the predictive value for high risk credit at 1% and high for low risk credit at 100%
 - Recall is 70% for high risk and 57% for low risk 


### Balanced Random Forest Classifier

 - Accuracy is 78.8%
 - Precision is low for the predictive value for high risk credit at 4% and high for low risk credit at 100%
 - Recall is 67% for high risk and 91% for low risk 


### Easy Ensemble Classifier

 - Accuracy is 92.5%
 - Precision is low for the predictive value for high risk credit at 7% and high for low risk credit at 100%
 - Recall is 91% for high risk and 94% for low risk 

## Summary

