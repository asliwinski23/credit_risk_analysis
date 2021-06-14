# credit_risk_analysis

## Project Overview
The POV for this project is that I am a data scientist for a bank. I am working with our internal mortgage team to evaluate future loan risk. To do so, I am testing a variety of machine learning models to see which will be the best to use in the future.

## Resources
Data Source: https://help.lendingclub.com/hc/en-us/articles/215488038-What-do-the-different-Note-statuses-mean-

Main Toolbox: python, Jupyter Notebook, sklearn libraries

## Results
The six machine learning models we ran are as follows:
* Naive Random Oversampling
* SMOTE Oversampling
* Cluster Centroids (undersampling)
* SMOTEENN (over and undersampling combination)
* Balanced Random Forest
* Easy Ensemble AdaBoost Classifier

Below is a comparison of accuracy, precision, and recall score amongst the models
#### Naive Random Oversampling

Accuracy: .884

Precision: .610

Recall: .780

#### SMOTE Oversampling

Accuracy: .882

Precision: .650

Recall: .780

#### Cluster Centroids

Accuracy: .883

Precision: .610

Recall: .780

#### SMOTEENN

Accuracy: 0.884

Precision: 0.53

Recall: 0.79

#### Balanced Random Forest

Accuracy: 0.991

Precision: .790

Recall: .890

#### Easy Ensemble AdaBoost Classifier
Accuracy: .991

Precision: .780

Recall: .920

## Summary
Based on these results it is clear to see that the Ensemble models, Balanced Random Forest and AdaBoost Classifier would be the recommended models to use in the future. Between the two, Balanced Random Forest would be my top recommendation because in it's confusion matrix there were only 52 false positives (52 accounts of incorrectly labeling high risk loans), whereas AdaBoost Classifier had 55. This may seem like a small distinction, but for this use case it is especially important to be conservative in labeling high risk loans. Furthermore, I am comfortable making this decision as the difference in the accuracy of the models is negligible.
