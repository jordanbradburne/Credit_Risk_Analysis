# Credit_Risk_Analysis

## Overview of the analysis: 
- Employ different techniques to train and evaluate models with unbalanced classes. Use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.
- Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. 
- Use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
- Compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Deliverables:
Deliverable 1: Use Resampling Models to Predict Credit Risk
Deliverable 2: Use the SMOTEENN Algorithm to Predict Credit Risk
Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk

## Results: 
### Naive Random Oversampling:
<img width="688" alt="Screen Shot 2021-10-17 at 10 41 28 PM" src="https://user-images.githubusercontent.com/85847344/137675099-563043fc-fa5c-428c-b6d2-06e0b77c9eb6.png">
* Accuracy: 0.67
* Precision (Avg): 0.99
* Recall: 0.61

### SMOTE Oversampling:
<img width="661" alt="Screen Shot 2021-10-17 at 10 42 44 PM" src="https://user-images.githubusercontent.com/85847344/137675175-9905046a-3092-480a-8a25-f64bc8acb782.png">
* Accuracy: 0.66
* Precision (Avg): 0.99
* Recall: 0.69

### Undersampling:
<img width="700" alt="Screen Shot 2021-10-17 at 10 43 46 PM" src="https://user-images.githubusercontent.com/85847344/137675252-1b3f8fd7-ad5a-4ae5-bee7-58eb77ca5476.png">
* Accuracy: 0.52
* Precision (Avg): 0.99
* Recall: 0.40

### Combination (Over and Under) Sampling:
<img width="670" alt="Screen Shot 2021-10-17 at 10 44 18 PM" src="https://user-images.githubusercontent.com/85847344/137675288-4a965480-4568-4df7-9647-65b8121cf9a6.png">
* Accuracy: 0.64
* Precision (Avg): 0.99
* Recall: 0.57

### Balanced Random Forest Classifier:
<img width="667" alt="Screen Shot 2021-10-17 at 10 45 24 PM" src="https://user-images.githubusercontent.com/85847344/137675376-0543591c-39a9-4f26-a9b5-157c5c92057c.png">
* Accuracy: 0.78
* Precision (Avg): 0.99
* Recall: 0.87

### Easy Ensemble AdaBoost Classifier
<img width="650" alt="Screen Shot 2021-10-17 at 10 46 13 PM" src="https://user-images.githubusercontent.com/85847344/137675451-01f16aad-1790-4764-b618-d457cda56920.png">
* Accuracy: 0.93
* Precision (Avg): 0.99
* Recall: 0.94

## Top ML Models: Performance Metrics

* Best Overall Balanced Accuracy Score: Easy Ensemble Classifer (93%)
* Best Overall Precision (high risk): Easy Ensemble Classifer (9%)
* Best Overall Recall: Easy Ensemble Classifer (94%)

## Summary: 
Every model used to perform the credit risk analysis show very low/weak precision in determining if the credit risk is high. The Easy Ensemble Classifier model shows a recall of about 93% which means that is detects almost all high risk credit. It has a very low precision so a lot of low risk credits are still falsely detected as high risk. This would cause issues with the bank's credit strategy and create difficulties on its revenue by missing these business opportunities. 
So I would not recommend that the bank use any of these models, but if they had to choose one I would say the Easy Ensemble Classifier.
