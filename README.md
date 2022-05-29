# Credit Risk Analysis
Challenge Module 17: Supervised Machine Learning and Credit Risk


## Project Overview
The number of credit cards issued by commercial banks is increasing and because of that customer credits risk issues receiver more attention and the concept of risk gives you a logical way to make the decision about whether or not to lend people the money. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, it is necessary to employ different techniques to train and evaluate models with unbalanced classes and because of this, the purpose of this project is to build, analyze and evaluate several machine learning models to predict credit card risk using the *imbalanced-learn* and s*cikit-learn* libraries to build and evaluate models using resampling.


## Resources
Data Source: LoanStats_2019Q1.csv
- Python 3.9.0
- Anaconda Navigator 2.1.1, Jupyter Notebook 6.4.6,

## Results
### Deliverable 1: Use Resampling Models to Predict Credit Risk
**Naive Random Oversampling**
- Balance accuracy score: 0.6403
- Generate a confusion matrix
<img src="/Resources/d1_cm1.png" width="30%" height="30%">

- Print out the imbalanced classification report.
<img src="/Resources/d1_icr1.png" width="50%" height="50%">

**SMOTE Oversampling**
- Balance accuracy score: 0.6515
- Generate a confusion matrix
<img src="/Resources/d1_cm2.png" width="30%" height="30%">

- Print out the imbalanced classification report.
<img src="/Resources/d1_icr2.png" width="50%" height="50%">

**Undersampling**
- Balance accuracy score: 0.5443
- Generate a confusion matrix
<img src="/Resources/d1_cm3.png" width="30%" height="30%">

- Print out the imbalanced classification report.
<img src="/Resources/d1_icr3.png" width="50%" height="50%">

------------------------------------------------------------------------------------------------------------------
### Deliverable 2: Use the SMOTEENN algorithm to Predict Credit Risk
**Combination (Over and Under) Sampling**
- Balance accuracy score: 0.6449
- Generate a confusion matrix
<img src="/Resources/d2_cm1.png" width="30%" height="30%">

- Print out the imbalanced classification report.
<img src="/Resources/d2_icr1.png" width="50%" height="50%">


------------------------------------------------------------------------------------------------------------------
### Deliverable 3: Use Ensemble Classifiers to Predict Credit Risk
**Balanced Random Forest Classifier**
- Balance accuracy score: 0.7885
- Generate a confusion matrix
<img src="/Resources/d3_cm1.png" width="30%" height="30%">

- Print out the imbalanced classification report.
<img src="/Resources/d3_icr1.png" width="50%" height="50%">

**Easy Ensemble AdaBoost Classifier**
- Balance accuracy score: 0.9317
- Generate a confusion matrix
<img src="/Resources/d3_cm2.png" width="30%" height="30%">

- Print out the imbalanced classification report.
<img src="/Resources/d3_icr2.png" width="50%" height="50%">


## Summary
Results of the machine learning models: ***High Risk***
| ML Model | Balance Accuracy Score | Precision | Recall | F1 |
| :---         |     :---:      |     :---:      |      :---:      |       ---: |
| Oversampling   | 0.64 | 0.01 | 0.66 | 0.02 |
| SMOTE    | 0.65 | 0.01 | 0.61 | 0.02 |
| Undersampling   | 0.54 | 0.01 | 0.69 | 0.01 |
| SMOTEENN    | 0.65 | 0.01 | 0.72 | 0.02 |
| Balanced Random Forest Classifier | 0.79 | 0.03 | 0.70 | 0.06 |
| Easy Ensemble AdaBoost Classifier | 0.93 | 0.09 | 0.92 | 0.16 |


Various techniques have been tried to handle class imbalance in a data set. The table above shows the results of the model for *high risk*, it can be observed, a relatively low accuracy when it comes to predicting high risk applicants. The highest one was the *Easy Ensemble AdaBoost Classifier* with 9% precision. This means that out of all the customers marked as *high risk* 9% were actually *high risk*.  

If our objective were to minimize company/banks loss, a good recall rate is desirable because we want to identify the maximum amount of clients that are indeed prone to stop paying their debts, in other words banks want to be able to mark all of the *high risk* clients as *high risk*. The highest recall when it comes to our data is when we run the *Easy Ensemble Adaboost Classifier* with a sensitivity of 92% which is pretty close to almost perfectly classifying the high-risk applicants. 

A low precision and high recall in the results means that the model detects the class well but also includes samples of other classes, and this also means that many people who were actually low risks were predicted hish risks and therfore might have been rejected.

In general observation, I cannot recommend using any of these models for the bank to use when determining *high risk* applicants due to the low F1-score rate we see throughout the analysis.  


