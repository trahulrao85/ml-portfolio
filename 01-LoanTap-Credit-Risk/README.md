# LoanTap — Personal Loan Credit Risk Model

## Business Problem
LoanTap is an online lending platform serving salaried professionals and MSMEs. 
The data science team needed an underwriting model to determine creditworthiness — 
specifically whether a credit line should be extended to an individual applicant.

## Dataset
- 39 features including loan amount, interest rate, employment length, 
  annual income, DTI ratio, credit history, and public records
- Target variable: Loan Status (Fully Paid vs Charged Off)

## Approach & Methodology
1. Exploratory Data Analysis — distribution plots, count plots, heatmaps
2. Feature Engineering — created binary flags for pub_rec, mort_acc, 
   pub_rec_bankruptcies
3. Missing value treatment and outlier handling
4. Scaling using MinMaxScaler
5. Logistic Regression model (Scikit-learn)
6. Evaluation via ROC-AUC curve, Precision-Recall curve, Classification Report

## Key Business Insight
Modeled the precision-recall tradeoff from a lender's perspective:
- High Recall priority = catch all defaulters, accept more false positives
- High Precision priority = only approve safe loans, miss some good borrowers
- Recommended threshold tuning based on NPA risk appetite

## Tools Used
Python | Pandas | NumPy | Scikit-learn | Matplotlib | Seaborn | Statsmodels

## Files
- `loantap_analysis.ipynb` — Full analysis notebook (coming soon)
