# Credit_Risk_Analysis

## Overview of the Analysis
Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.

## Results: 

### RandomOverSampler Model
![first](Mod17_photos/m17_6.png)
* The balanced accuracy score is 65%.
* The high_risk precision is about 1% only with 62% sensitivity which makes a F1 of 2% only.
* Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 68%.

### SMOTE Model
![second](Mod17_photos/m17_5.png)
* The balanced accuracy score is 64%.
* The high_risk precision is about 1% only with 63% sensitivity which makes a F1 of 2% only.
* Due to the high number of the low_risk population, its precision is almost 100% with a sensitivity of 66%.

### ClusterCentroids Model
![third](Mod17_photos/m17_4.png)
* The balanced accuracy score is down to about 52%.
* The high_risk precision is still 1% only with 63% sensitivity which makes a F1 of 1%
* Due to the high number of false positives, the low_risk sensitivity is only 40%.

### SMOTEENN Model
![fourth](Mod17_photos/m17_3.png)
* The balanced accuracy score is about 62%.
* The high_risk precision is still 1% only with 68% sensitivity which makes a F1 of only 2%.
* Due to the high number of false positives, the low_risk sensitivity is 57%.

### BalancedRandomForestClassifier Model
![fifth](Mod17_photos/m17_2.png)
* The balanced accuracy score improved to about 79%.
* The high_risk precision is still low at 4% only with 67% sensitivity which makes a F1 of only 7%.
* Due to a lower number of false positives, the low_risk sensitivity is now 91% with 100% presicion.

### EasyEnsembleClassifier Model
![sixth](Mod17_photos/m17_1.png)
* The balanced accuracy score is high to about 93%.
* The high_risk precision is still low at 7% only with 91% sensitivity which makes a F1 of only 14%.
* Due to a lower number of false positives, the low_risk sensitivity is now 94% with 100% presicion.

## Summary 
In conclusion, I would not recommend the bank to use any of these models to predict credit risk. All the models used to perform the credit risk analysis display weak precision in determining if a credit risk is high.
The Ensemble models showed the most improvement, specifucally on the sensitivity of the high risk credits.
The EasyEnsembleClassifier model displays a recall of 92%, so it detects almost all high risk credit. However with a low precision, a lot of low risk credits are still falsely detected as high risk which would penalize the bank's credit strategy and infer on its revenue by missing those business opportunities.
