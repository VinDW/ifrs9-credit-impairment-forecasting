# IFRS 9 Credit Impairment Forecasting Model

## Project Overview

This project develops an IFRS 9-style credit impairment forecasting model using Python. The model estimates probability of default, loss given default, exposure at default and expected credit loss for a synthetic retail banking loan portfolio.

The project demonstrates how statistical modelling can support credit-risk analytics, impairment forecasting, portfolio segmentation and financial risk monitoring in a banking environment.

## Business Problem

Banks need to estimate expected credit losses on loan portfolios for impairment reporting, pricing, capital planning and credit-risk management. Expected credit loss modelling combines the probability that a borrower may default, the expected loss if default occurs and the exposure outstanding at the time of default.

This project provides a simplified portfolio-level framework for estimating expected credit loss and analysing how impairment differs across borrower risk grades.

## Methodology

Expected credit loss is calculated as:

```text
ECL = PD × LGD × EAD
```

where:

- `PD` is the probability of default.
- `LGD` is the loss given default.
- `EAD` is the exposure at default.
- `ECL` is the expected credit loss.

The modelling workflow includes:

1. Generating a synthetic retail banking loan portfolio.
2. Creating borrower-level credit-risk features.
3. Simulating loan default behaviour.
4. Training a logistic regression probability of default model.
5. Evaluating model performance using accuracy, ROC-AUC and a confusion matrix.
6. Estimating borrower-level probability of default.
7. Assigning loss given default assumptions by risk grade.
8. Using loan amount as the exposure at default proxy.
9. Calculating expected credit loss.
10. Summarising impairment by risk grade.

## Repository Structure

```text
ifrs9-credit-impairment-forecasting/
│
├── data/
│   └── synthetic_credit_portfolio.csv
│
├── figures/
│   ├── roc_curve_pd_model.png
│   ├── total_ecl_by_risk_grade.png
│   └── impairment_ratio_by_risk_grade.png
│
├── notebooks/
│   └── 01_ifrs9_impairment_model.ipynb
│
├── outputs/
│   ├── model_metrics.csv
│   ├── impairment_summary.csv
│   └── ecl_by_risk_grade.csv
│
├── README.md
└── requirements.txt
```

## Folder Descriptions

### `data`

Contains the synthetic retail banking loan portfolio used in the project.

### `notebooks`

Contains the Jupyter Notebook used to generate the portfolio data, train the probability of default model, calculate expected credit loss and produce the final outputs.

### `figures`

Contains visual outputs from the project, including the ROC curve, total expected credit loss by risk grade and impairment ratio by risk grade.

### `outputs`

Contains the final model and portfolio summary tables, including model performance metrics, portfolio impairment summary and expected credit loss by risk grade.

## Tools Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- Jupyter Notebook

## Key Results

The probability of default model achieved a ROC-AUC score of approximately 0.70, showing reasonable ability to distinguish between lower-risk and higher-risk borrowers.

The impairment analysis showed that higher-risk grades produced higher expected credit loss ratios, which is consistent with credit-risk theory and banking portfolio behaviour.

## Project Outputs

The project produces the following outputs:

- Synthetic retail banking loan portfolio
- Probability of default model metrics
- Portfolio impairment summary
- Expected credit loss by risk grade
- ROC curve for the probability of default model
- Total expected credit loss chart by risk grade
- Impairment ratio chart by risk grade

## Skills Demonstrated

This project demonstrates practical skills in:

- Credit-risk modelling
- Probability of default estimation
- Expected credit loss calculation
- IFRS 9-style impairment forecasting
- Logistic regression modelling
- Portfolio segmentation
- Model evaluation
- Financial risk analytics
- Banking data science

## Relevance to Quantitative Analyst Roles

This project is relevant to banking quantitative analyst roles because it demonstrates the ability to build and explain models used for impairment forecasting, credit-risk assessment, financial modelling and portfolio risk monitoring.

## Author

Vincent Kometsi
