## 🌲 Task 5: Predictive Modeling

## Overview

This project was completed as part of the **BCG X Data Science Job Simulation** on **Forage**.

The objective was to build and evaluate a predictive model for customer churn using the cleaned and engineered PowerCo dataset, and to determine which features actually drive churn.

---

## Business Scenario

With a dataset of cleaned and engineered features from Task 4, the next step was to see how well those features could predict whether a customer would churn. Estelle recommended a **Random Forest classifier** — a supervised learning algorithm well suited to this kind of classification problem.

A Random Forest makes predictions by building many decision trees on different samples of the data and taking a majority vote across them to decide on a final prediction.

---

## Approach

### 1. Prepare the Data

- Used the final modeling dataset, `data_for_predictions.csv`, prepared by Estelle after a further review of the engineered features.
- Split the data into training and test sets, separating the churn label (target) from the predictor features.

### 2. Train the Model

- Trained a **Random Forest Classifier** (scikit-learn) to predict customer churn based on the engineered features.

### 3. Evaluate the Model

Chose **Accuracy, Precision, and Recall** as evaluation metrics, rather than accuracy alone, because churn is an imbalanced target — only around 10% of customers in the dataset actually churned. A model that simply predicted "no churn" for everyone would still score a high accuracy while being useless in practice, so precision and recall were needed to understand how well the model actually identified churners.

**Results on the test set:**

| Metric | Score |
|---|---|
| Accuracy | 90.4% |
| Precision | 81.8% |
| Recall | 4.9% |

| | Predicted: No Churn | Predicted: Churn |
|---|---|---|
| **Actual: No Churn** | 3,282 (TN) | 4 (FP) |
| **Actual: Churn** | 348 (FN) | 18 (TP) |

### 4. Interpret the Results

- The model is very good at identifying customers who will **not** churn, but performs poorly at catching customers who **will** churn — of the 366 customers who actually churned in the test set, the model only caught 18 of them.
- This low recall means the model, in its current form, is **not yet reliable enough** to drive a retention program on its own — more work is needed on feature engineering and model tuning to reduce false negatives.

### 5. Feature Importance

- Plotted a feature importance chart to identify which engineered features actually contributed to the model's predictions.
- **Net margin** and **12-month consumption** emerged as the most important predictors of churn.
- The price-sensitivity features engineered in Task 4 were scattered in importance and did **not** stand out as a main driver of churn in their current form — directly informing the business recommendation that followed in Task 6.

---

## Key Skills Demonstrated

- Supervised machine learning (Random Forest classification)
- Train/test splitting and model evaluation
- Selecting evaluation metrics appropriate to an imbalanced classification problem
- Interpreting confusion matrices, precision, and recall
- Feature importance analysis and translating it into a business insight

---

## Deliverables

- [`data_for_predictions.csv`](./data_for_predictions.csv) — final modeling dataset
- [`modeling_starter.ipynb`](./modeling_starter.ipynb) — starter notebook template
- [`Modeling_Answer.ipynb`](./Modeling_Answer.ipynb) — completed modeling and evaluation notebook

---

## Learning Outcomes

Through this task, I gained hands-on experience with:

- Building and training a Random Forest classifier using scikit-learn
- Choosing evaluation metrics appropriate for an imbalanced target variable
- Critically assessing whether a model's performance is "good enough" for a business use case, not just reporting a single accuracy number
- Using feature importance to test a business hypothesis (price sensitivity) rather than assuming it
