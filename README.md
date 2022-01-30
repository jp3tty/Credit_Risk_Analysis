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


### SMOTE Oversampling

The balanced accuracy of SMOTE oversampling is 0.66.

SMOTE oversampling confusion matrix:
![CM_SMOTEOversampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_SMOTE_Oversampling.PNG)

SMOTE oversampling classification report:
![ClassReport_SMOTEOversampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassReport_SMOTE_Oversampling.PNG)


### Undersampling

The balanced accuracy of undersampling is 0.54.

Undersampling confusion matrix:
![CM_Undersampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_Undersampling.PNG)

Undersampling classification report:
![ClassReport_Undersampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassRepot_Undersampling.PNG)


### Combination Sampling

The balanced accuracy of combination sampling is 0.67.

Combination sampling confusion matrix:
![CM_CombinationSampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_Combined.PNG)

Combination sampling classification report:
![ClassReport_CombinationSampling](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassReport_Combined.PNG)


### Balanced Random Forest Classifier

The balanced accuracy of random forest classifier is 0.79.

Balanced random forest classifier confusion matrix:
![CM_BRFC](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_BalancedRandomForestClassifier.PNG)


Balanced random forest classifier classification report:
![ClassReport_BRFC](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassRepot_BalancedRandomForestClassifier.PNG)


### Easy Ensemble AdaBoost Classifier

The balanced accuracy of easy ensemble adaboost classifier is 0.93.

Easy ensemble AdaBoost classifier confusion matrix:
![CM_EEAC](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ConfusionMatrix_EasyEnsembleAdaBoostClassifier.PNG)

Easy ensemble AdaBoost classifier classification report:
![ClassReport_EEAC](https://github.com/jp3tty/Credit_Risk_Analysis/blob/main/Images/ClassReport_EasyEnsembleAdaBoostClassifier.PNG)



* There is a bulleted list that describes the balanced accuracy score and the precision and recall scores of all six machine learning models



## Summary
The models used to perform the risk analysis show weak precision in determining high credit risk. 

* There is a summary of the results
* There is a recommendation on which model to use, or there is no recommendation with a justification