# Credit Risk Analysis with Logistic Regression

## Overview

This repository contains code for a credit risk analysis project using logistic regression. The purpose of this analysis is to develop a machine learning model to predict whether a loan is healthy or has a high risk of defaulting based on various financial attributes.

## Dependencies

Make sure you have the following dependencies installed:

```bash
conda show scikit-learn
```

## Dataset

The dataset used for this analysis is stored in the `lending_data.csv` file located in the `Resources` folder. The dataset contains the following columns:

- `loan_amnt`: Loan amount
- `int_rate`: Interest rate
- `annual_inc`: Annual income
- `dti`: Debt-to-income ratio
- `emp_length`: Employment length
- `loan_status`: Target variable indicating loan status (0: healthy loan, 1: high-risk loan)

## Model Training and Evaluation

We trained logistic regression models using the training data and evaluated their performance using accuracy, precision, and recall metrics.

## Results

The main results of the analysis are as follows:

- Accuracy: 99%
- Precision (class 0): 100%
- Precision (class 1): 86%
- Recall (class 0): 100%
- Recall (class 1): 91%

## References

- [University of Adelaide Git bootcamp](https://git.bootcampcontent.com/University-of-Adelaide/UADEL-VIRT-DATA-PT-12-2023-U-LOLC/-/tree/main/20-Supervised-Learning?ref_type=heads)
- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Scikit-Learn Documentation](https://scikit-learn.org/stable/documentation.html)
