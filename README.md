# Predicting_Credit_Card_Fraud
Predicting credit card fraud with multiple linear and non-linear models
### Overview
The Annual Data Book compiled by the Federal Trade Commission reports that Credit card fraud accounted for 393,207 of the nearly 1.4 million reports of identity theft in 2020. This makes credit card fraud the second most common type of identity theft reported, behind only government documents and benefits fraud for that year. Some surveys suggest that a typical organization loses 5% of their yearly revenues to fraud. These numbers can only increase since the number of non-cash transactions increases provides more opportunities for credit card fraud.

For retailers and banks to not lose money, procedures must be put in place to detect fraud prior to it occurring.
Credit card companies must identify fraudulent credit card transactions so that customers are not charged for items that they did not purchase. To combat this problem, financial institution traditionally uses rule-based approaches to identify fraudulent transactions. These algorithms use strict rules to determine when a transaction is fraudulent.

#### Some challenges of a strict rule-based algorithm include:

=======
* Any new scenario that could lead to fraud needs to be manually coded into the algorithm
* Increases in customers and size of data leads to a corresponding increase in the human effort, time and cost required to track new scenarios and update the algorithm
* Since the algorithm cannot go beyond defined rules, it cannot dynamically recognize new scenarios that could result in fraudulent transaction.

To overcome these limitations, organizations are beginning to utilize machine learning and data science to build fraud detection systems. Given the size of available data, computational resources, and powerful machine learning algorithm available today, data science and machine learning processes will be able to find patterns in data and detect frauds easily.

#### The Dataset

The goal of this Credit Card Fraud Detection project is to classify a transaction as valid or fraudulent in a large dataset. Since we are dealing with discrete values, this is a binary classification problem, and we would employ the use of a supervised machine learning algorithm.
The dataset used contains transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced; the positive class (frauds) account for 0.172% of all transactions. 
The dataset contains only numerical input variables which are the result of a PCA transformation which was done to deidentify and anonymize the dataset for confidentiality issues. Features V1, V2, ... V28 are the extracted features obtained with PCA, the only features which have not been transformed with PCA are ‘Time’ and ‘Amount’. 
Feature ‘Time’ contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature ‘Amount' is the transaction Amount. Feature 'Class' is the response variable, and it takes value 1 in case of fraud and 0 otherwise.

#### Initial Approach

The is an imbalanced dataset. The imbalance between classes is compensated using oversampling and under sampling. The logistic regression, random forest, support vector machine, k-means are used within a cross-validation framework. Lastly, recall and accuracy are considered as metrics while choosing the best classifier.

### Control Flow
      1.	Understanding the problem
      2.	Importing required libraries and understanding their use
      3.	Importing data and learning its structure
      4.	Performing basic EDA
      5.	Scaling different variables
      6.	Outlier treatment
      7.	Building basic Classification model with Random Forest
      8.	Nearmiss technique for under sampling data
      9.	SMOTE for oversampling data
      10.	cross validation in the context of under sampling and oversampling
      11.	Pipelining with sklearn/imblearn
      12.	Applying Linear model: Logistic Regression
      13.	Applying Ensemble technique: Random Forest
      14.	Applying Non-Linear Algorithms: Support Vector Machine, Decision Tree, and k-Nearest Neighbor
      15.	Making predictions on test set and computing validation metrics
      16.	ROC curve and Learning curve
      17.	Comparison of results and Model Selection
      18.	Visualization with seaborn and matplotlib
