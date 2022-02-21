# Credit Risk Analysis

## Overview of the Analysis

The imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling.  A credit card dataset from LendingClub was used to oversample and undersample data using RandomOverSampler, SMOTE, and ClusterCentroids algorithms.  SMOTEENN was used for the combination approach of over and undersampling.  Finally two machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, that reduce bias were used to predict credit risk.

## Results


### Random Oversampling

 - Accuracy is 63.7%
 - Precision is low for the predictive value for high risk credit at 1% and high for low risk credit at 100%
 - Recall is 62% for high risk and 65% for low risk
  
![RandomOversampling_Accuracy](https://user-images.githubusercontent.com/90982811/155032528-c4b76bb6-cf82-4082-b592-96ce4a639057.jpg)

![RandomOversampling_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155032548-0144796c-1741-4b6e-8dd3-3213cf9f6a55.jpg)

### SMOTE Oversampling

 - Accuracy is 63%
 - Precision is low for the predictive value for high risk credit at 1% and high for low risk credit at 100%
 - Recall is 62% for high risk and 64% for low risk 

![SMOTEOversampling_Accuracy](https://user-images.githubusercontent.com/90982811/155032558-6e687d8b-3c8b-47c6-90d8-aa5b13525029.jpg)

![SMOTEOversampling_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155032563-e3d8f1d3-77eb-46ee-ae51-42b810b13214.jpg)

### ClusterCentroids Undersampling

 - Accuracy is 63%
 - Precision is low for the predictive value for high risk credit at 1% and high for low risk credit at 100%
 - Recall is 62% for high risk and 64% for low risk 

![ClusterCentroidsUndersampling_Accuracy](https://user-images.githubusercontent.com/90982811/155032574-35ebd7e6-a429-4480-843d-14f06ad063b1.jpg)

![ClusterCentroidsUndersampling_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155032588-1b49719e-93b4-4a88-98fe-3d92b1b68754.jpg)

### SMOTEENN Over and Under Sampling

 - Accuracy is 63.8%
 - Precision is low for the predictive value for high risk credit at 1% and high for low risk credit at 100%
 - Recall is 70% for high risk and 57% for low risk 

![SMOTEENN_Accuracy](https://user-images.githubusercontent.com/90982811/155032611-e086106a-e809-4c55-8fa2-94138045bf8e.jpg)

![SMOTEENN_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155032669-18c1de97-4fae-4054-90ad-d08960c3988c.jpg)

### Balanced Random Forest Classifier

 - Accuracy is 78.8%
 - Precision is low for the predictive value for high risk credit at 4% and high for low risk credit at 100%
 - Recall is 67% for high risk and 91% for low risk 

![BRFC_Accuracy](https://user-images.githubusercontent.com/90982811/155032684-08662db2-d915-4c15-a740-525e72518a5d.jpg)

![BRFC_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155032693-de5f0fd9-5d10-4846-8931-00b2c117de38.jpg)

### Easy Ensemble Classifier

 - Accuracy is 92.5%
 - Precision is low for the predictive value for high risk credit at 7% and high for low risk credit at 100%
 - Recall is 91% for high risk and 94% for low risk 
 
![EasyEnsembleClassifier_Accuracy](https://user-images.githubusercontent.com/90982811/155032735-d62e9e92-f5ac-4508-bef1-4e5593c7a946.jpg)

![EasyEnsembleClassifier_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155032766-95ae1232-ca0a-4bf6-9ddc-fef373e25074.jpg)

## Summary

The four oversampling and undersampling models returned low accuracy scores.  In addition, the precision for high risk credit within these models was only 1% with unimpressive recall rates.

The Balanced Random Forest Classifier returned a higher accuracy rate of 78.8%, a higher precision for high risk credit at 4%, and higher recall rates.

The Easy Ensemble Classifier returned the highest all around results with 92.5% accuracy.  The model is accurate at returning true positives with 91% recall for high risk credit and 94% for low risk credit.  The precision has been consistent across all models returning 100% performance for low risk credit.  The Easy Ensemble Classifier returned the highest predictive value for high risk credit with a 7% precision rate.  Since the precision is so low for accurately predicting high risk credit, it is recommended that the lending service compare this precision rate against industry standards.  The lending service may not want to rely on a model that turns that many customers away if they were flagged a high risk but in fact were not, however predicting credit is complex.  If the precision rate is within industry standard, I would recommend the Easy Ensemble Classifier since it has the overall best results with accuracy and recall scores.  If this is not within industry standard, I recommend searching for a model that returns better precision rates for high risk credit.
