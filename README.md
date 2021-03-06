# credit_risk_analysis
## Overview of the analysis:
Jill commends you for all your hard work. Piece by piece, you’ve been building up your skills in data preparation, statistical reasoning, and machine learning. You are now ready to apply machine learning to solve a real-world challenge: credit card risk.

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, you’ll need to employ different techniques to train and evaluate models with unbalanced classes. Jill asks you to use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling.

Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, you’ll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, you’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, you’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once you’re done, you’ll evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results:
Cobination:
* Accuracy Score:.65
* Precison Score:The precision for the high-risk is low about 1% and for low-risk precision is high 100%.
* Recall Score:The recall value for high-risk is slightly higher than the low-risk (70 and 58 respectively)
![com](https://github.com/allisonorourke-ufGfGy/credit_risk_analysis/blob/main/Linear_regression/images/Combination.png)

SMOTE:
* Accuracy Score:.66
* Precison Score:The precision for the high-risk is low about 1% and for low-risk precision is high 100%.
* Recall Score: The recall value for high-risk is slightly higher than the low-risk (63 and 69 respectively)
![smote](https://github.com/allisonorourke-ufGfGy/credit_risk_analysis/blob/main/Linear_regression/images/smote1.png)

RandomOverSample:
* Accuracy Score:.65
* Precison Score:The precision for the high-risk is low about 1% and for low-risk precision is high 100%.
* Recall Score:The recall value for high-risk is slightly higher than the low-risk (74 and 55 respectively).
![random](https://github.com/allisonorourke-ufGfGy/credit_risk_analysis/blob/main/Linear_regression/images/Naive%20Rnadom%20Oversampling.png)

Undersampling:
* Accuracy Score:.54
* Precison Score: The precision for the high-risk is low about 1% and for low-risk precision is high 100%.
* Recall Score: The recall value for high-risk is higher than the low-risk (67 and 42 respectively).
![cluster](https://github.com/allisonorourke-ufGfGy/credit_risk_analysis/blob/main/Linear_regression/images/uNDERSAMPLING%201.png)

BalancedRandomForestClassifier:
* Accuracy Score:.79
* Precison Score:The precision for the high-risk is low about 3% and for low-risk precision is high 100%.
* Recall Score:The recall value for high-risk is higher than the low-risk(87 and 70 respectively).
![Balanced](https://github.com/allisonorourke-ufGfGy/credit_risk_analysis/blob/main/Linear_regression/images/BalancedRandomForestClassifier.png)

EasyEnsembleClassifier:
* Accuracy Score:.93
* Precison Score:The precision for the high-risk is low about 9% and for low-risk precision is high 100%.
* Recall Score:The recall value for high-risk and low-risk are very similar  (92 and 94 respectively).
![Easy](https://github.com/allisonorourke-ufGfGy/credit_risk_analysis/blob/main/Linear_regression/images/EasyEnsembleClassifer.png)

## Summary:
The data shows that it is very hard for the machiene learning to predict credit-risk. Overall, I would liekly advise against the use of any of the algorithims. The EasyEnsembleClassifer model has the higher overall accuracy score with a .93 but this was probably due to the fact that the data was unbalanced. Even when it's balanced accuracy and average F-score were above .90 , it's F-score for high-risk prediction was no better than 0.16. With something as important as credit-score I just feel like this would put individuals too at risk to not be able to accuratly predict who is actually high risk.
