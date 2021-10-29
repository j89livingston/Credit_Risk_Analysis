# Credit Risk Analysis

![https://github.com/jvera01/-Credit_Risk_Analysis-/raw/main/Resources/B1.PNG](https://github.com/jvera01/-Credit_Risk_Analysis-/raw/main/Resources/B1.PNG)

## <b>Project Overview</b>
We were hired by a peer-to-peer lending service company called LendingClub to oversample data using their credit card dataset. We will oversample the data using: 

- RandomOverSampler and SMOTE algorithms, 
- Undersample using ClusterCentroids 
- Combinational approach of under and over sampling using the SMOTEENN algorithm. 

Using two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.
___
## <b>Resources</b>
Software: Visual Studio Code, Jupyter Notebook/Labs, Python 3.7

Data Source: LoanStats_2019Q1.csv

___
## <b>Results</b>

### RandomOverSampling:
* Balance Accuracy Score: 64%
* Precision: 0.99
* Recall Score:0.61

<img src="Resources/ROS.png" alt="Resources/ROS.png" width="600"/>

----

### SMOTE:
* Balance Accuracy Score: 66%
* Precision: 0.99
* Recall Score: 0.69

<img src="Resources/SMOTE.png" alt="Resources/SMOTE.png" width="600"/>

----

### UnderSampling with ClusterCentoids:
* Balance Accuracy Score: 66%
* Precision: 0.99
* Recall Score: 0.41

<img src="Resources/CC.png" alt="Resources/CC.png" width="600"/>

----

### SMOTEENN:
* Balance Accuracy Score: 55%
* Precision: 0.99
* Recall Score: 0.58

<img src="Resources/SMOTEENN.png" alt="Resources/SMOTEENN.png" width="600"/>

----

### Balanced Random Forest Classifier:
* Balance Accuracy Score: 79%
* Precision: 0.99
* Recall Score: 0.87

<img src="Resources/BRFC.png" alt="Resources/BRFC.png" width="600"/>

----

### Easy Ensemble AdaBoost Classifier:
* Balance Accuracy Score: 93%
* Precision: 0.99
* Recall Score: 0.94

<img src="Resources/ESC.png" alt="Resources/ESC.png" width="600"/>

----
## <b>Summary</b>

The randomoversampling, SMOTE, ClusterCentoids, and SMOTEENN did not perform well enough for a credit risk environment. The undersampling, oversampling and a combination all performed between 55%-66%. This is too low and inconsistent to be used. The Balance Random Forest Classifier could be usable, running at a Balance Accuracy Score of 79%. The best Classifier would be the Easy Ensemble Adaboost classifier, running with a balance score of 93% and 0.99 precision.

After factoring in these three main statistics, the model that I would recommend to use for predicting high-risk loans is the Easy Ensemble Classifying model. This model has the highest recall rate for high-risk loans and the highest accuracy score. The recall rate for high-risk loans is important because it shows how many high-risk loans are being flagged as high risk. Accuracy is also important because you want to make sure that the model is not flagging too many low-risk loans as high risk. This model has both of these statistics in its favor, making it the best model for this scenario.

The main advantage of the ensemble method is that it can overcome the limitations of the base classifiers. In the same way, it can achieve a better classification accuracy than the base classifiers. The main disadvantage of the ensemble method is that it requires a lot of computational resources. It is because the decision trees are trained and tested in parallel in each iteration. The analisis shows the comparison of accuracy between the Easy Ensembled Adaboost and the SMOTE Oversampling.

- Naive Random Oversampling (64%)

- SMOTE Sampling (66%)

- ClusterCentoids Undersampling (66%)

- SMOTEENN Sampling (55%)

- Balanced Random Forest Classifying (79%)

- Easy Ensemble Classifying (93%)


In conclusion, I created a machine learning model to determine whether or not a loan would be granted based on several different factors. I then tested this model against a test dataset and found that it was able to correctly identify low and high risk loans with an accuracy rate. This shows that this machine learning model can be used in practice to accurately identify which loans should be approved and which should not be approved based on their level of risk. This is important because it means that this machine learning model can be used in practice to accurately identify which loans should be granted and which should not be granted, which saves money for the bank by only approving the most profitable loans while rejecting the less profitable ones. This is important because it means that this machine learning model can be used in practice to accurately identify which loans should be granted and which should not be granted, which saves money for the bank by only approving the most profitable loans while rejecting the less profitable ones.
