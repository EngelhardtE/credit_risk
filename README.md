# credit_risk

## Overview

The purpose of this project is to demonstrate how to use several different models in order to predict credit risk and evaluate their effectiveness. This includes:

- Resampling Models: RandomOverSampler, SMOTE algorithms, and ClusterCentroids algorithms
- SMOTEENN algorithms
- Ensemble Classifiers: BalancedRandomForestClassifier and EasyEnsembleClassifier 

## Results

### RandomOverSampler

- Balanced Accuracy Score: 65%
- Precision: 99%
- Recall Score: 67%

![RandomOverSampler](Resources/RandomOverSampler.png)

### SMOTE

- Balanced Accuracy Score: 63%
- Precision: 99%
- Recall Score: 63%

![SMOTE](Resources/SMOTE.png)

### ClusterCentroids

- Balanced Accuracy Score: 63%
- Precision: 99%
- Recall Score: 45%

![ClusterCentroids](Resources/ClusterCentroids.png)

### SMOTEENN

- Balanced Accuracy Score: 51%
- Precision: 99%
- Recall Score: 56%

![SMOTEENN](Resources/SMOTEENN.png)

### BalancedRandomForestClassifier

- Balanced Accuracy Score: 79%
- Precision: 99%
- Recall Score: 91%

![BalancedRandomForestClassifier](Resources/BalancedRandomForestClassifier.png)

### EasyEnsembleClassifier

- Balanced Accuracy Score: 93%
- Precision: 99%
- Recall Score: 94%

![EasyEnsembleClassifier](Resources/EasyEnsembleClassifier.png)

## Summary

All of the methods listed have a precision of 99%, but they differ when it comes to their recall rates. A high recall rate means that the method is more efficient at catching high risk loans, but it also means that there is a higher chance of falsely flagging a low-risk loan as high risk. A low recall rate means that the method is less efficient at catching high risk loans, but also produces false positives. 

By this logic, whether one method is better than the other is up to the institution using it and their level of risk tolerance. High risk tolerance would allow for a low recall rate (ClusterCentroids) as it would maximize the number of loans made but maximize the risk of unintentionally making a high-risk loan. A low risk tolerance would require a high recall rate (EasyEnsembleClassifier) as it would minimize the chance of unintentionally making a high-risk loan at the cost of a lower overall number of loans made. 

While you can hypothetically say that no one method is truly the best for all loaning institutions, it is likely that most would prefer a high recall rate to stay on the safer side. Even if fewer loans are made, the diminished chance of making a high-risk loan and having to face the recipient defaulting is a favorable outcome. Therefore, a method like EasyEnsembleClassifier will likely fit a loan institution’s risk strategy more often than not.
