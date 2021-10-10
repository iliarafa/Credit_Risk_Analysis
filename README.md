# Credit_Risk_Analysis
## Project Overview

The purpose of this project is to build and evaluate models using resampling. We are dealing with credit and 
when dealing with credit, we are dealing with an inherently unbalanced classification problem, as good loans easily outnumber risky loans.
Therefore, we will employ different techniques to train and evaluate models with unbalanced classes and conclude which if any model can be used to predict credit risk. 

# Results
# Accuracy, Precision and Recall Scores
## NaiveRandomOversampling

<img src="Resources/images/naive_random_os.png" width="722" height="123" /><br><br>
**Accuracy Score :** 0.65<br>
**Precision score :** 0.99<br>
**Recall score :** 0.68


## SMOTE Oversampling
<img src="Resources/images/smote_os.png" width="722" height="123" /><br><br>
**Accuracy Score :** 0.62<br>
**Precision score :** 0.99<br>
**Recall score :** 0.64



## ClusterCentroids
**Accuracy Score :** 0.53<br><br>
<img src="Resources/images/cluster_os.png" width="722" height="123" /><br><br>
**Accuracy Score :** 0.53<br>
**Precision score :** 0.99<br>
**Recall score :** 0.45


## SMOTEENN

<img src="Resources/images/smoteenn_os.png" width="722" height="123" /><br><br>
**Accuracy Score :** 0.64<br>
**Precision score :** 0.99<br>
**Recall score :** 0.58


## BalancedRandomForestClassifier

<img src="Resources/images/forest_os.png" width="722" height="123" /><br><br>
**Accuracy Score :** 0.64<br>
**Precision score :** 0.99<br>
**Recall score :** 0.87


## EasyEnsembleClassifier

<img src="Resources/images/ensemble_os.png" width="722" height="123" /><br><br>
**Accuracy Score :** 0.93<br>
**Precision score :** 0.99<br>
**Recall score :** 0.92


## Summary 

Out of the six models we evalueated, five show accuracy scores between 53% and 65%. **NaiveRandom** and **SMOTE** Oversampling, **Cluster Centroids** and **SMOTEENN** also show poor results in their recall scores. Because of this combination of low accuracy and recall scores these four models should not be prefered to predict credit risk. Moving forward, the **BalancedRandomForestClassifier** counters the low accuracy score (64%) with a fair recall score of 87%. This makes the model more balanced but still not ideal for our purpose. Last but not least, the **EasyEnsembleClassifier** scores an amazing 93% in accuracy while also scoring 92% in recall. This is a very accurate and trustworthy model that can be used to predict credit risk. 
