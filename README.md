# Credit_Risk_Analysis

## Overview of the Analysis

This project seeks to employ and analyze different machine learning models that will help to predict credit risk. The models employed are BalancedRandomForestClassifier, EasyEnsembleClassifier,oversampling and undersampling algorithms. Since credit risk is a an unbalanced classification problem, this project uses different techniques to train and  evaluate models with unbalanced classes.In this file we will analyze how the models performed based on accuracy, precision and recall, to make a recommendation on which machine learning model to use for predicting credit risk.


## Results


### Balanced Random Forest Clasiffier
 * Balanced accuracy score: 87%
 * Precision: the precision for high risk loans is very small(3%) while the precision for the low-risk loans is of 100%. This indicates that the model correctly predicted low-risk all of the time but was not so good at predicting high-risk loans.
 * Recall: the recall for both low-risk and high-risk loans is fairly good, above 70%. This means that the model is good at predicting true positives for both types of loans especifically for low-risk loans.
 !()[Resources/Balanced_Random_Forest.png)

### Easy Ensemble Balanced Classifier
 * Balanced accuracy score: 79%
 * Precision: the precision for high risk loans is very small less than 10% while the precision for the low-risk loans is of 100%. This indicates that the model correctly predicted low-risk all of the time but was not so good at predicting high-risk loans.
 * Recall: the recall for both low-risk and high-risk loans is very good, above 90%. This means that the model is good at predicting true positives for both types of loans and it actually very good at identifying high-risk loans.


### Naive Random Oversampling
 * Balanced accuracy score: 67%
 * Precision: the precision for high risk loans is very bad around 1% while the precision for the low-risk loans is of 100%. This indicates that the model correctly predicted low-risk all of the time but was not so good at predicting high-risk loans.
 * Recall: the recall for both low-risk and high-risk loans is fairly good, above 70%. This means that the model is good at predicting true positives for both types of loans especifically for low-risk loans.

### SMOTE Oversampling
 * Balanced accuracy score: 66%
 * Precision: the precision for high risk loans is very bad around 1% while the precision for the low-risk loans is of 100%. This indicates that the model correctly predicted low-risk all of the time but was not so good at predicting high-risk loans.
 * Recall: the recall for both low-risk and high-risk loans is about 60%. This means that the model can predict true positives for both types of loans but not that good.

### Undersampling
 * Balanced accuracy score: 66%
 * Precision: the precision for high risk loans is very bad around 1% while the precision for the low-risk loans is of 100%. This indicates that the model correctly predicted low-risk all of the time but was not so good at predicting high-risk loans.
 * Recall: the recall for high risk loans is almost 70% while the recall for low-risk loans is 40%. This means that the model is better at predicting high-risk loans than low-risk loans, which is good for the purpose of the project but 70% is still not that good. 

## Summary
As we can see from the previous machine learning model results, there are some models that have a good balanced accuracy score but that does not necessarily indicates that it will be a good model. In this case the most important parameter taken into account to make a recommendation on which model to use is recall, because this tell us how good or bad the model was at predicting high-risk loans. Easy Ensemble Balanced Classifier performed the best, it has a recall of 92% in predicting high-risk loans and 94% recall at predicting low-risk loans. It is important to mentioned that this model does not performed so well on precision, meaning that only 1% of the time the model was not so good at predicting positives. 
