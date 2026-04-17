# Credit Risk Classification

## Overview
A logistic regression model built to predict loan risk for a peer-to-peer lending 
company. Using historical lending data, the model classifies borrowers as either 
healthy (low-risk) or high-risk, helping financial institutions make more informed 
lending decisions.

---

## Features Used
- Loan size
- Interest rate
- Borrower income
- Debt-to-income ratio
- Number of accounts
- Derogatory marks
- Total debt

**Target variable:** `loan_status` — 0 (healthy loan) or 1 (high-risk loan)

---

## Model Performance

| Metric | Healthy Loan (0) | High-Risk Loan (1) |
|--------|-----------------|-------------------|
| Precision | 100% | 86% |
| Recall | 100% | 91% |
| F1-Score | 1.00 | 0.88 |
| **Overall Accuracy** | | **99%** |

---

## Summary
The logistic regression model performs exceptionally well overall, achieving 99% 
accuracy. It identifies healthy loans with perfect precision and recall, and 
correctly flags 91% of actual high-risk loans. For most lending use
