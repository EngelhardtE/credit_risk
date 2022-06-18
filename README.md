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
