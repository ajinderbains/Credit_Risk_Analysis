# Credit Risk Analysis

## Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, we will  employ different techniques to train and evaluate models with unbalanced classes.

We will ll oversample the data using:

1. RandomOverSampler 
2. SMOTE algorithms

We will undersample the data using: 

3. ClusterCentroids algorithm
4. SMOTEENN(Combination of Over and Under Sampling)

We will also  compare two new machine learning models to  reduce bias:

5. BalancedRandomForestClassifier 
6. EasyEnsembleClassifier

## Results
1. Accuracy,Precision and Recall score from **RandomOverSampler** algorithm
   - Accuracy score = 0.65
   - Precision Score = 0.99
   - Recall Score = 0.59
   
![chart1](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/ROSA-1.png)
![chart2](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/ROSpr-1.png)

2. Accuracy,Precision and Recall score from **SMOTE** algorithm
   - Accuracy score = 0.66
   - Precision Score = 0.99
   - Recall Score = 0.68
   
![chart3](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/Sma-2.png)
![chart4](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/smpr-2.png)

3. Accuracy,Precision and Recall score from **ClusterCentroids** algorithm
   - Accuracy score = 0.65
   - Precision Score = 0.99
   - Recall Score = 0.42

![chart5](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/usa-3.png)
![chart6](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/uspr-3.png)

4. Accuracy,Precision and Recall score from **SMOTEENN** algorithm
   - Accuracy score = 0.65
   - Precision Score = 0.99
   - Recall Score = 0.57

![chart7](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/uosa-4.png)
![chart8](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/uospr-4.png)

5. Accuracy,Precision and Recall score from **BalancedRandomForestClassifier** algorithm
   - Accuracy score = 0.78
   - Precision Score = 0.99
   - Recall Score = 0.89
   
![chart9](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/brfca-5.png)
![chart10](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/brfcpr-5.png)

6. Accuracy,Precision and Recall score from **EasyEnsembleClassifier** algorithm
   - Accuracy score = 0.93
   - Precision Score = 0.99
   - Recall Score = 0.94
 
![chart11](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/eeca-6.png)
![chart12](https://github.com/ajinderbains/Credit_Risk_Analysis/blob/main/images/eecpr-6.png)

## Summary

If Accuracy,precision and recall score is close to  1.0 means that every result retrieved by a search was relevant .
- Accuracy score for all algorithms is **0.65** except **EasyEnsembleClassifier** which has **0.93**.
- Precision score for all algorithms is **0.99**
- Recall score varies for all algorithms from 0.42 to 0.78 but **EasyEnsembleClassifier** algorithm is **0.94**

So to predict which algorothms is best then we have to consider the results of accuracy,precision and recall together.We have also calculated the values of F1 score which inclide the values of precision and recall in calculations.
For **EasyEnsembleClassifier** algorithm :
   - Accuracy score = 0.93
   - Precision Score = 0.99
   - Recall Score = 0.94
   
 which are very close and if we find F1 score = 0.97 ,which is very close to ideal value 1.So I recommend the  **EasyEnsembleClassifier** algorithm .
 
