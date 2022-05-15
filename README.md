# ANDROID-AUTHENTICITY-PREDICTION

# Introduction

In recent years, smartphones have brought people’s lives to a new high level. Smartphone applications, or Apps, are accelerating the process with many more functions getting developed, such as browsing the Internet, making payments, taking photos and share. However, the "Apps" are bringing potential vulnerability when they access private information from the phones, and mobile security has never been so much focused on like today. 
We used different machine learning models like Logistic regression, Decision Tress, Random Forest, Gradient Boosting, XGBoost, KNN and Naïve bayes using cross validation  approach for predicting whether the app is benign or malware. Multiple evaluation indices such as Precision, Recall, F1-Score, ROC-AUC Score  are used to measure the prediction performance of the classification models.

# Problem Statement

This dataset consists of apps needed permissions during installation and run-time. We collect apps from three different sources google play, third-party apps and malware dataset. This file contains more than 30,000 Android apps. features extracted at the time of installation and execution. One file contains the name of the features and others contain .apk file corresponding to it extracted permissions with respective package. Apps are collected from Google's play store, hiapk, app china, Android, mumayi , gfan slideme, and pandaapp. These .apk files collected from the last three years continuously and contain 81 distinct malware families. But, Here you are only supposed to predict whether the app is benign (0) or malware(1).

We have the following variables in the dataset: 
1. Class :- Whether the app is Benign(0) or Malware(1) :-
2. App :- Name of the App
3. Package :- OBB/Data package installed in root folder
4. Category :- App Category (eg. Entertainment, Adventure, puzzle, Action, Antivirus, etc.)
5. Description :- App Description
6. Rating :- Rating out of 5
7. Number of ratings :- No. of Ratings given by users
8. Price :- Price of the App
9. Related apps:- Apps related to installed App
10. Dangerous (D) permissions count :- No. of Dangerous Permissions allowed by user
11. Safe (S) permissions count :- No. of Safe Permissions allowed by user
12. Default: Access DRM content. (S) :- 0 : No , 1 : Yes
11. Phone calls: modify phone state (S) :- 0 : No , 1 : Yes

We have shown only a part of the features since there are 184 total features

# Steps Involved 
1. Installing libraries and gathering the dataset
2. Pre-processing the dataset: - Checking for Missing values, Duplicate values etc.
3. Exploratory Data Analysis: - Analysing the dependent variable, categorical and numerical variables individually.
4. Feature Engineering: - Creation of new features according to our need, dropping of unnecessary data points or features by checking correlation, VIF etc., handling of outliers, One–Hot Encoding and normalization of features.
5. Fitting of Machine Learning models with training dataset and evaluating with testing dataset: - like Linear regression, Decision Tress, Random Forest, Gradient Boosting
6. Hypertuning and Explaining the best model with LIME and ELI5

# Models Used
1. Logistic Regression
2. Decision tree
3. Random Forest
4. Gradient Boost
5. KNN
6. Naive Bayes
7. XGBoost

Out of which, Logistic Regression had the best F1 score for testing dataset. Hence we will select this model and find the best hyper parameters for it.






