# Credit_Risk_Analysis
## Overview
This analysis aims to classify a loan applicant as a good loan or a risky loan, considering that most loan applicants are good loans. 

Logistical regression is performed balanced samples made with RandomOverSampler, SMOTE, ClusterCentroids, SMOTEENN, BalancedRandomForestClassifier, and EasyEnsembleClassifier.

## Results
### RandomOverSampler
![](/images/RandomOverSampler.png)
 - Balanced Accuracy Score: 0.63
 - Precision of high-risk loans: 0.01
 - Recall of high-risk loans: 0.61

 ### SMOTE
 ![](/images/SMOTE.png)
 - Balanced Accuracy Score: 0.62
 - Precision of high-risk loans: 0.01
 - Recall of high-risk loans: 0.55

 ### ClusterCentroids
 ![](/images/ClusterCentroids.png)
 - Balanced Accuracy Score: 0.52
 - Precision of high-risk loans: 0.01
 - Recall of high-risk loans: 0.60

 ### SMOTEENN
 ![](/images/SMOTEENN.png)
 - Balanced Accuracy Score: 0.61
 - Precision of high-risk loans: 0.01
 - Recall of high-risk loans: 0.66

 ### BalancedRandomForestClassifier
 ![](/images/BalancedRandomForestClassifier.png)
 - Balanced Accuracy Score: 0.72
 - Precision of high-risk loans: 0.03
 - Recall of high-risk loans: 0.56

 ### EasyEnsembleClassifier
 ![](/images/EasyEnsembleClassifier.png)
 - Balanced Accuracy Score: 0.89
 - Precision of high-risk loans: 0.08
 - Recall of high-risk loans: 0.84

 ## Summary
 In terms of the balanced accuracy score, only the BalancedRandomForestClassifier and EasyEnsembleClassifier performed better than 0.7, with the three oversampling/undersampling algorithms had less than 0.7 scores.

 The oversampling/undersampling algorithms also had only a precision of 0.01, showing them wholy unfit to classify high-risk loans. Although the BalancedRandomForestClassifier and EasyEnsembleClassifier performed better with precisions of 0.03 and 0.08, respectively, and the EasyEnsembleClassifier managed to catch 0.84 of the high-risk loans, they are still shown to overwhelmingly predict loans as low-risk.