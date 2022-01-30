# Credit_Risk_Analysis

## Overview
Machine learning is a method of data analysis that automates analytical model building. The following exercise uses machine learning (ML) techniques to assess credit risk of an inherently unbalanced class distribuition of good loans against risky loans.


## Results
"Loan status" entries were used from the "LoanStats_2019Q1" dataset to train a number of ML models for determining whether a credit applicantion should be considered high or low risk. Predictions were preformed for each and they were compared for accuracy, precision, and recall.

### Naive Random Oversampling

The balanced accuracy of naive random oversampling is 0.65.

Naive random oversampling confusion matrix:
![CM_NaiveRandomOversampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_NaiveRandomOversample.PNG)

Naive random oversampling classification report:
![ClassReport_NaiveRandomOversampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassReport_NaiveRandomOversample.PNG)

The report shows:
* High risk precision of 1% with a recall of 71%, giving this model an F1 score of 2%.
* Low risk precision of 100% and a recall of 58%.


### SMOTE Oversampling

The balanced accuracy of SMOTE oversampling is 0.66.

SMOTE oversampling confusion matrix:
![CM_SMOTEOversampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_SMOTE_Oversampling.PNG)

SMOTE oversampling classification report:
![ClassReport_SMOTEOversampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassReport_SMOTE_Oversampling.PNG)

The report shows:
* High risk precision of 1% with a recall of 63%, giving this model an F1 score of 2%.
* Low risk precision of 100% and a recall of 68%.



### Undersampling

The balanced accuracy of undersampling is 0.54.

Undersampling confusion matrix:
![CM_Undersampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_Undersampling.PNG)

Undersampling classification report:
![ClassReport_Undersampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassRepot_Undersampling.PNG)

* High risk precision of 1% with a recall of 69%, giving this model an F1 score of 1%.
* Low risk precision of 100% and a recall of 40%.


### Combination Sampling

The balanced accuracy of combination sampling is 0.67.

Combination sampling confusion matrix:
![CM_CombinationSampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_Combined.PNG)

Combination sampling classification report:
![ClassReport_CombinationSampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassReport_Combined.PNG)

* High risk precision of 1% with a recall of 73%, giving this model an F1 score of 2%.
* Low risk precision of 100% and a recall of 60%.


### Balanced Random Forest Classifier

The balanced accuracy of random forest classifier is 0.79.

Balanced random forest classifier confusion matrix:
![CM_BRFC](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_BalancedRandomForestClassifier.PNG)


Balanced random forest classifier classification report:
![ClassReport_BRFC](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassRepot_BalancedRandomForestClassifier.PNG)

* High risk precision of 3% with a recall of 70%, giving this model an F1 score of 6%.
* Low risk precision of 100% and a recall of 87%.


### Easy Ensemble AdaBoost Classifier

The balanced accuracy of easy ensemble adaboost classifier is 0.93.

Easy ensemble AdaBoost classifier confusion matrix:
![CM_EEAC](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_EasyEnsembleAdaBoostClassifier.PNG)

Easy ensemble AdaBoost classifier classification report:
![ClassReport_EEAC](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassReport_EasyEnsembleAdaBoostClassifier.PNG)

* High risk precision of 9% with a recall of 92%, giving this model an F1 score of 16%.
* Low risk precision of 100% and a recall of 94%.


## Summary
All the models used to perform the risk analysis show weak precision in determining high credit risk. The best result from these machine learning models was the Easy Ensemble AdaBoost Classifier with an accuracy rate of 93% and a precision of 9% when predicting high risk candidates. The recall (or sensitivity) of this model was also the highest at 92%. Based on these results I would recommend the Easy Ensemble AdaBoost Classifier.
