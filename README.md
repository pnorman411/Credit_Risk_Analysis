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

The four oversampling and undersampling models returned low accuracy scores.  In addition, the precision for high risk credit within these models was only 1% with unimpressive recall rates.

The Balanced Random Forest Classifier returned a higher accuracy rate of 78.8%, a higher precision for high risk credit at 4%, and higher recall rates.

The Easy Ensemble Classifier returned the highest all around results with 92.5% accuracy.  The model is accurate at returning true positives with 91% recall for high risk credit and 94% for low risk credit.  The precision has been consistent across all models returning 100% performance for low risk credit.  The Easy Ensemble Classifier returned the highest predictive value for high risk credit with a 7% precision rate.  Since the precision is so low for accurately predicting high risk credit, it is recommended that the lending service compare this precision rate against industry standards.  The lending service may not want to rely on a model that turns that many customers away if they in fact were not a high risk, however predicting credit is complex.  If the precision rate is within industry standard, I would recommend the Easy Ensemble Classifier since it has the overall best results with accuracy and recall scores.