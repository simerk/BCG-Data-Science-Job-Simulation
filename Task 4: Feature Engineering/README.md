## 🛠️ Task 4: Feature Engineering

## Overview

This project was completed as part of the **BCG X Data Science Job Simulation** on **Forage**.

The objective was to engineer new features from PowerCo's cleaned client and price data to better capture the drivers of customer churn — in particular, to test Estelle's hypothesis that the **difference between off-peak prices in December and the preceding January** could be a significant predictor of churn.

---

## Business Scenario

Having analyzed the influence of price sensitivity on churn in Task 3, the next step was to enrich the dataset itself. Estelle, the senior data scientist on the case, suggested that seasonal price differences — rather than raw price levels — might carry more predictive signal. My task was to build this feature, and to continue engineering additional features to prepare the dataset for modeling.

---

## What Is Feature Engineering?

Feature engineering refers to the **addition, deletion, combination, or mutation** of a dataset to improve machine learning model training, leading to better performance and accuracy. In this context, it meant engineering the price and client data into new columns that would help predict churn more accurately — grounded in a sound understanding of the business problem.

---

## Approach

### 1. Remove Redundant Columns

- Reviewed each column for relevance, checking for columns with only one unique value or columns that were near-duplicates of others, and removed those that added no analytical value.

### 2. Build Estelle's Suggested Feature

- Engineered the **difference between off-peak energy prices in December vs. the preceding January**, to directly test whether seasonal price swings relate to churn.

### 3. Expand on Price Variation Features

- Built an **average price change** feature, measuring the average price difference by company across peak, mid-peak, and off-peak periods.
- Built a **maximum price change** feature, capturing the largest price difference across periods and months — another lens on how much a customer's bill fluctuates seasonally.
- Rationale: large seasonal price swings (e.g. a winter bill spike) are a plausible trigger for a customer to shop around for a better deal.

### 4. Date & Categorical Transformations

- Converted date columns into numeric components (e.g. month) and dropped the raw date columns, since machine learning models require numeric input.
- Converted boolean columns into binary (0/1) values.
- Converted categorical columns into dummy variables (one-hot encoding).

### 5. Skew Correction

- Revisited the skewed distributions identified during EDA and applied a **log transformation** to bring them closer to a normal distribution, since many modeling techniques assume normally distributed inputs.

### 6. Correlation Analysis & Pruning

- Plotted a correlation matrix across all features to identify highly correlated columns.
- Removed columns that were strongly correlated with others, since they were likely holding redundant information.

---

## Key Skills Demonstrated

- Feature engineering (creation, transformation, and selection)
- Hypothesis-driven feature design
- Date/categorical/boolean encoding for machine learning
- Skew correction via log transformation
- Correlation analysis and multicollinearity reduction

---

## Deliverables

- [`clean_data_after_eda.csv`](./clean_data_after_eda.csv) — cleaned dataset carried forward from Task 3
- [`feature_engineering.ipynb`](./feature_engineering.ipynb) — starter notebook template
- [`Feature_Engineering_Answer.ipynb`](./Feature_Engineering_Answer.ipynb) — completed feature engineering notebook

---

## Learning Outcomes

Through this task, I gained hands-on experience with:

- Translating a stakeholder's hypothesis into an engineered feature
- Designing features that capture business-relevant behavior (seasonal price variation) rather than just raw values
- Preparing categorical, boolean, and date data for machine learning
- Using log transformations to address skew
- Using correlation analysis to reduce redundancy before modeling
