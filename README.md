# Credit Card Fraud Detection


## Problem Statement : 
Credit card fraud causes significant financial loss and requires high-recall, low-latency detection systems. The challenge lies in severely imbalanced data and minimizing false negatives while maintaining precision. 
## Solution Overview : 
Built an end-to-end supervised ML pipeline to detect fraudulent transactions. The system includes robust preprocessing, imbalance handling using SMOTE, and model benchmarking to identify the best trade-off between recall and precision. 
## Approach : 
### 1. Data Understanding & EDA :
Analyzed transaction patterns and fraud distribution
Identified strong predictors and correlations
### 2. Data Preprocessing : 
Feature scaling and cleaning
Train-test split with stratification
### 3. Imbalance Handling : 
Applied SMOTE to address ~20% class imbalance 
Improved minority class learning and recall
### 4. Modeling : 
Logistic Regression (baseline) 
Decision Tree 
Random Forest (final model)
### 5. Evaluation : 
Precision, Recall, F1-Score
AUC-ROC for threshold-independent performance
## Results & Impact : 
Random Forest outperformed baseline models Significant improvement in fraud recall after SMOTE 
Balanced precision-recall trade-off suitable for real-world fraud systems
## Tech Stack used: 
Python 
Pandas, NumPy
Scikit-learn
Matplotlib, Seaborn
imbalanced-learn (SMOTE)
## Key Engineering Takeaways : 
Handling imbalanced data is critical for production ML Recall is a business-critical metric in fraud detection
Model selection should align with domain cost functions
