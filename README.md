# Credit Risk Analysis

## Overview of the Analysis

The imbalanced-learn and scikit-learn libraries were used to build and evaluate models using resampling.  A credit card dataset from LendingClub was used to oversample and undersample data using RandomOverSampler, SMOTE, and ClusterCentroids algorithms.  SMOTEENN was used for the comination approach of over and undersampling.  Finally two machine learning models, BalancedRandomForestClassifier and EasyEnsembleClassifier, that reduce bias were used to predict credit risk.

## Results



### Random Oversampling

![RandomOversampling_Accuracy](https://user-images.githubusercontent.com/90982811/155026067-af60d9db-f12f-4f1d-86da-1a31dddb46dd.jpg)

![RandomOversampling_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155026081-af0a7027-796a-4458-bd63-fecb6851b10d.jpg)

### SMOTE Oversampling

![SMOTEOversampling_Accuracy](https://user-images.githubusercontent.com/90982811/155026104-1165f706-8a00-493e-9934-53ea6e49b498.jpg)

![SMOTEOversampling_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155026117-f1c1d236-5244-4758-a3ed-ed27469e37b8.jpg)

### ClusterCentroids Undersampling

![ClusterCentroidsUndersampling_Accuracy](https://user-images.githubusercontent.com/90982811/155026131-a58042e0-eac7-45b7-9e24-8f316e3074c3.jpg)

![ClusterCentroidsUndersampling_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155026140-392b8aa5-f35a-4717-ac83-dcae30405bda.jpg)

### SMOTEENN Over and Under Sampling

![SMOTEENN_Accuracy](https://user-images.githubusercontent.com/90982811/155026160-9bfcd2cf-08f4-4122-86ab-c153a91f041f.jpg)

![SMOTEENN_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155026166-62858e4d-c0e7-41d4-85c8-32e73c7d12f5.jpg)

### Balanced Random Forest Classifier

![BRFC_Accuracy](https://user-images.githubusercontent.com/90982811/155026173-8493ba44-1136-4a1f-9a3f-6c6e87352965.jpg)

![BRFC_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155026180-0c41975c-041e-470b-bc5f-feba82fa2d0e.jpg)

### Easy Ensemble Classifier

![EasyEnsembleClassifier_Accuracy](https://user-images.githubusercontent.com/90982811/155026208-74921723-987e-47fb-bf0f-8837891f94a2.jpg)

![EasyEnsembleClassifier_ImbalancedClassificationReport](https://user-images.githubusercontent.com/90982811/155026226-1872732f-755f-4ab0-bc39-e2b58687cb23.jpg)

## Summary

