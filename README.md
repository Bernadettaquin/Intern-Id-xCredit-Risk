IDX Partners – Credit Risk Prediction

A machine learning project aimed at predicting credit default risk using demographic and financial data from loan applicants between 2018–2023. This project helps optimize loan approval decisions through data-driven insights.

Dataset Overview
Total Records: 19,158 loan applicants
Time Period: 2018–2023
Target Variable:
Label 0 (Low Risk: 86.28%)
Label 1 (High Risk: 13.72%)

Business Objective: To predict the risk of loan default using historical applicant data. The insights support loan underwriting decisions by identifying high-risk applicants based on financial behavior and demographic profiles.

Exploratory Data Analysis (EDA) with Key Features: loan_amnt, funded_amnt, interest_rate, dti, total_pymnt, recoveries, annual_inc, etc.

Key Findings:
1.Larger loan amounts, higher interest rates, and high DTI are correlated with higher default risk.
2.Recoveries is highly variable—indicating uneven loan recoverability.
3.Annual income contains significant outliers but is weakly correlated with loan amount.

Data Quality & Preprocessing
Missing Values: Removed columns with >50% missing; filled numerical columns with median, categorical with mode.
Encoding: All categorical features encoded for ML compatibility.
Outliers: Identified in annual_inc, installment, etc., and handled appropriately.
Feature Engineering: Added loan_to_income_ratio for improved model relevance.

Models Compared:
1.Logistic Regression
2.Decision Tree Classifier
3.✅ Random Forest Classifier (Best performance)

Data Splitting & Scaling: Train-Test Split
Feature scaling using StandardScaler for better model stability

Feature Importance (Top Predictors)
recoveries: ~0.35–0.40
term: ~0.20–0.25
int_rate: ~0.15–0.20
revol_bal: ~0.05–0.10
installment: ~0.05–0.10
loan_to_income_ratio: ~0.05–0.10

Insight: Relative debt burden (e.g., loan-to-income ratio) is a more reliable indicator than absolute income.

Business Recommendations
1. Strengthen recovery strategies for non-performing loans.
2. Impose stricter conditions for long-term loans.
3. Calibrate interest rates to reflect borrower risk profiles.
4. Enforce thresholds for debt ratios like revol_bal and loan_to_income_ratio.
5. Integrate feature importance insights into the credit approval system.

This project uses supervised learning to improve credit risk assessment by identifying critical financial behavior patterns. The result: more accurate loan approval processes and reduced financial risk.





