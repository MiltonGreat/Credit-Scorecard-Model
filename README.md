# Credit Scorecard Model

![screenshot-localhost_8888-2025 04 01-12_44_45](https://github.com/user-attachments/assets/e03a7061-d93d-47ce-a2b5-223b884f5db0)

### Project Overview

This project focuses on developing a credit scorecard model to assess an individual's creditworthiness based on financial features such as credit history, purpose, and savings. The model utilizes Weight of Evidence (WoE) and Information Value (IV) to transform categorical and numerical features into meaningful predictive variables, followed by logistic regression for credit risk assessment.

The scorecard is designed to provide an interpretable and data-driven approach to credit scoring, which can be used in financial lending and risk evaluation.

### Dataset

The dataset contains financial and demographic information related to credit applicants. The key features used in this model include:

- Credit History – Previous loan repayment behavior.
- Purpose – The reason for applying for credit.
- Savings – Amount of savings available.
- Amount – Loan amount requested.
- Duration – Loan repayment period.

The target variable is Credit Risk (Good/Bad Credit), where 1 represents bad credit and 0 represents good credit.

### Methodology

The project follows a structured approach to building a credit scorecard:

1. Data Preprocessing – Handling missing values, feature encoding, and binning.
2. Feature Engineering – Using Weight of Evidence (WoE) transformation and selecting features based on Information Value (IV).
3. Logistic Regression Benchmark – Establishing a baseline model.
4. Credit Scorecard Development – Assigning points based on feature contributions and computing final scores.
5. Model Evaluation – Assessing performance using AUC-ROC, AUC-PR, KS Statistic, and Confusion Matrix.

### Results

1. Model Performance:
- AUC-ROC: 0.6739
- AUC-PR: 0.8028
- Balanced Accuracy: 0.5512
- KS Statistic: 30.71%

2. Classification Report:
- High recall for bad credit cases (effective in detecting defaulters).
- Lower recall for good credit cases (misclassification of non-defaulters).
- Score bands calculation encountered challenges (empty bins).

### Future Improvements

To enhance model accuracy and reliability:

- Improve feature selection by incorporating additional financial indicators.
- Optimize binning strategies to resolve empty score bands.
- Balance precision-recall for better classification of good credit cases.
- Explore alternative models such as boosting algorithms for better predictive performance.

### Conclusion

This project successfully implemented a credit scorecard model using logistic regression, WoE transformation, and score-based risk assessment. Despite moderate performance (AUC-ROC: 0.6739), the framework provides an interpretable approach to credit scoring. Future refinements will focus on improving feature selection, fine-tuning binning, and enhancing recall for good credit cases.

### Source

![German Credit Data from Kaggle](https://www.kaggle.com/datasets/varunchawla30/german-credit-data)
