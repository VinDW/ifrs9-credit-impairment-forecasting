# IFRS 9 Credit Impairment Forecasting Model

## Project Overview

This project develops an IFRS 9-style credit impairment forecasting model using Python. 
The aim is to estimate expected credit losses for a synthetic retail banking loan portfolio 
using probability of default (PD), loss given default (LGD), and exposure at default (EAD).

The project is designed to demonstrate quantitative modelling skills relevant to banking, 
including credit-risk modelling, impairment forecasting, portfolio segmentation, 
financial analytics, and model performance evaluation.

## Business Problem

Banks need to estimate potential credit losses on loan portfolios for impairment reporting, 
pricing, capital planning, and risk management. Under an expected credit loss framework, 
credit losses are estimated before default occurs by combining borrower-level default risk, 
loss severity, and outstanding exposure.

## Methodology

The expected credit loss is calculated as:

ECL = PD × LGD × EAD

where:

- PD is the probability of default;
- LGD is the loss given default;
- EAD is the exposure at default.

The project follows these steps:

1. Generate a synthetic retail banking loan portfolio.
2. Create borrower-level risk variables.
3. Estimate probability of default using logistic regression.
4. Estimate LGD using recovery-rate assumptions.
5. Estimate EAD using outstanding loan exposure.
6. Calculate expected credit loss.
7. Segment impairment by risk grade.
8. Evaluate model performance using accuracy, ROC-AUC, confusion matrix and classification report.

## Tools Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Key Outputs

- Borrower-level probability of default estimates
- Expected credit loss estimates
- Impairment summary by risk grade
- Model performance metrics
- Portfolio-level impairment estimate

## Relevance to Quantitative Analyst Role

This project demonstrates skills in:

- Credit-risk modelling
- Financial modelling
- Impairment forecasting
- Statistical modelling
- Forecasting and budgeting
- Model evaluation
- Banking portfolio analytics
- Clear communication of quantitative results
