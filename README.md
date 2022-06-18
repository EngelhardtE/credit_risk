# credit_risk

## Overview

The purpose of this project is to demonstrate how to use machine learning and different models in order to predict credit risk. Each model's effectiveness will then be evaluated to see if they can be reliably used to detect high-risk loans. The models to be tested include:

- Resampling Models: RandomOverSampler, SMOTE algorithms, and ClusterCentroids algorithms
- SMOTEENN algorithms
- Ensemble Classifiers: BalancedRandomForestClassifier and EasyEnsembleClassifier 

## Results

All of the models tested had near perfect low-risk precision, but varied in all other metrics. 

### RandomOverSampler

- Balanced Accuracy Score: 65%
- High-Risk Precision: 1%
- Recall Score: 67%

![RandomOverSampler](Resources/RandomOverSampler.png)

### SMOTE

- Balanced Accuracy Score: 63%
- High-Risk Precision: 1%
- Recall Score: 63%

![SMOTE](Resources/SMOTE.png)

### ClusterCentroids

- Balanced Accuracy Score: 63%
- High-Risk Precision: 1%
- Recall Score: 45%

![ClusterCentroids](Resources/ClusterCentroids.png)

### SMOTEENN

- Balanced Accuracy Score: 51%
- High-Risk Precision: 1%
- Recall Score: 56%

![SMOTEENN](Resources/SMOTEENN.png)

### BalancedRandomForestClassifier

- Balanced Accuracy Score: 79%
- High-Risk Precision: 4%
- Recall Score: 91%

![BalancedRandomForestClassifier](Resources/BalancedRandomForestClassifier.png)

### EasyEnsembleClassifier

- Balanced Accuracy Score: 93%
- High-Risk Precision: 7%
- Recall Score: 94%

![EasyEnsembleClassifier](Resources/EasyEnsembleClassifier.png)

## Summary

All the methods listed have a low-risk precision of 99%, but high-risk precision of less than 10%. They also differ greatly in their recall rates. Precision measures how accurate a test result is. Therefore, a low high-risk precision means that there is a low chance that a loan tested as high-risk is truly high-risk. On the other hand, recall measures the chance that a loan that is high-risk will be labeled as such. 

In this case, a high recall is more important than a high precision because a loan institution's biggest concern is detecting high-risk loans so that they do not loan money to borrowers who are likely to default. Even if some low-risk loans are wrongly flagged as high-risk, the loaning institution would likely value safety from default greatly. In other words, a false positive is better than a false negative. 

However, given the results a loaning institution would not even have to choose between prioritizing precision versus recall, as the EasyEnsembleClassifier method has the highest levels of both compared to the other five methods tested. 94% recall is quite high, although 7% high-risk precision leaves a lot of room for improvement. Of the methods tested, it is clearly the best option. It would likely be wise to perform further testing on other methods to see if one can be found with a comparable recall but with a higher high-risk precision.
