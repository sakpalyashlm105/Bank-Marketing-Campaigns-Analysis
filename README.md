# Bank-Marketing-Campaigns-Analysis

### Overview
This code performs exploratory data analysis and modeling on the Bank Marketing dataset from the UCI Machine Learning Repository [Link for dataset]([url](http://archive.ics.uci.edu/dataset/222/bank+marketing)). The goal is to predict if a client will subscribe to a term deposit based on features like age, job, marital status, education, balance, previous contacts, etc.

### Data
The dataset contains 45211 rows and 17 columns, including the target column 'y' indicating term deposit subscription. There is a class imbalance with the majority class ('no' term deposit subscription) having 39922 examples and the minority class ('yes') having 5289 examples.

### Analysis
The analysis includes:

* Loading and inspection of the data
* Visual EDA on numerical features like histograms, boxplots, CDF plots
* Analysis of feature distributions by target value for categorical features
* Data cleaning by removing outliers
* Upsampling minority class to handle class imbalance
* Encoding categorical features
* Feature correlation analysis
* Modeling using Decision Tree, Random Forest, XGBoost
* Evaluation with train/test splits, confusion matrix, classification report
* Feature importance analysis

### Key Insights
* Duration of contact is most highly correlated with target
* Upsampling helped improve model performance on minority class
* Random Forest had best performance with 97.5% accuracy
* Top features were duration, contact type, previous outcomes
