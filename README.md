# <font color=#6495ED>Credit Risk Analysis</font>

## <font color=#6495ED>Project Overview</font>

Fast lending, a peer to peer lending services comapny, wants to use machine learning to predict credit risk. We believe that machine learning will lead to more accurate identification of good candidates for loans which will lead to lower default rates. we will employ different techniques to build, train and evaluate several machine learning models with unbalanced classes,so that we can predict credit risk.

### <font color=#6495D>Purposes</font>

- Oversample the data using the **RandomOverSampler** algorithm.

- Oversample the data using the **RandomOverSampler** algorithm.

- Undersample the data using the **ClusterCentroids** algorithm.

- Over and undersampling using the **SMOTEENN** algorithm.

- Compare two new machine learning models that reduce bias, **BalancedRandomForestClassifier** and **EasyEnsembleClassifier**, to predict credit risk

## <font color=#6495ED>Resources</font>

### <font color=#6495D>Data Source: </font>
LoanStats_2019Q1.csv - credit card credit dataset from LendingClub, a peer-to-peer lending services company

### <font color=#6495D>Software:</font> 
- Anaconda with python 3.9
- Jupyter Notebook
- imbalanced-learn library (0.9.0) 
- scikit-learn library (1.1.1)

## <font color=#6495ED>Results</font> 
### Naive Random Oversampling

![Naive_Random_Oversampling](https://github.com/NingYang2022/Credit_Risk_Analysis/blob/main/images/Naive_Random_Oversampling.png?raw=true)

1. Balanced Accuracy: 63.13%
2. Precision: 1% for High-risk loans and 100% for Low-risk loans.
3. Recall: High/Low risk = 61% / 65%

### SMOTE Oversampling

![SMOTE_Oversampling](https://github.com/NingYang2022/Credit_Risk_Analysis/blob/main/images/SMOTE_Oversampling.png?raw=true)

1. Balanced Accuracy: 64.66%
2. Precision: 1% for High-risk loans and 100% for Low-risk loans.
3. Recall: High/Low risk = 63% / 66%

### Cluster Centroids Undersampling

![Cluster_Centroids_Undersampling](https://github.com/NingYang2022/Credit_Risk_Analysis/blob/main/images/Cluster_Centroids_Undersampling.png?raw=true)

1. Balanced Accuracy: 52.92%
2. Precision: 1% for High-risk loans and 100% for Low-risk loans.
3. Recall: High/Low risk = 61% / 45%

### SMOTEENN Over and Under Sampling

![SMOTEENN_Over_and_Under_Sampling](https://github.com/NingYang2022/Credit_Risk_Analysis/blob/main/images/SMOTEENN_Over_and_Under_Sampling.png?raw=true)

1. Balanced Accuracy: 63.76%
2. Precision: 1% for High-risk loans and 100% for Low-risk loans.
3. Recall: High/Low risk = 70% / 57%

### Balanced Random Forest Classifier

![Balanced_Random_Forest_Classifier](https://github.com/NingYang2022/Credit_Risk_Analysis/blob/main/images/Balanced_Random_Forest_Classifier.png?raw=true)

1. Balanced Accuracy: 78.71%
2. Precision: 4% for High-risk loans and 100% for Low-risk loans.
3. Recall: High/Low risk = 67% / 91%

### Easy Ensemble AdaBoost Classifier

![Easy_Ensemble_AdaBoost_Classifier](https://github.com/NingYang2022/Credit_Risk_Analysis/blob/main/images/Easy_Ensemble_AdaBoost_Classifier.png?raw=true)

1. Balanced Accuracy: 92.54%
2. Precision: 7% for High-risk loans and 100% for Low-risk loans.
3. Recall: High/Low risk = 91% / 94%

## <font color=#6495ED>Summary</font>

For all models for the credit card data set, the **Easy Ensemble AdaBoost Classifier** is the best model  with its 92.54% balanced accuracy. The precision for all models were similar and within an appropriate range. The **Easy Ensemble AdaBoost Classifier** also had the highest recall score, making it the most effective machine learning model for overall credit card analysis.
