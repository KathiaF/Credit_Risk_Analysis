# Credit Risk Analysis
Challenge Module 17

## Project Overview

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
