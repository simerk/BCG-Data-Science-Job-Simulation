# BCG X Data Science Job Simulation – Forage

This repository contains my solutions for the **BCG X Data Science Virtual Job Simulation** offered by **Forage**.

---

## Overview

The simulation provides practical experience with real-world data science consulting projects inspired by the work of BCG X's Data Science team. Working on behalf of a fictional energy company, **PowerCo**, the simulation covers the full analytics lifecycle — from framing a business problem and forming a hypothesis, through exploratory data analysis, feature engineering, and predictive modeling, to communicating findings and recommendations to senior stakeholders.

The core business question: **is customer churn being driven by price sensitivity, and if so, what should PowerCo do about it?**

---

## Repository Structure

### 📂 [Task 1 – Business Understanding](./Task%201)
Reviewed the business context and client request from PowerCo, understanding the churn problem from a business perspective and identifying what data and analysis would be needed to investigate it.

### 📂 [Task 2 – Problem Framing & Hypothesis](./Task%202)
Framed the business problem as a testable hypothesis — does price sensitivity drive customer churn? — and outlined a data-driven approach for investigating it, including what data was needed and how it would be analyzed.

### 📂 [Task 3 – Exploratory Data Analysis](./Task%203)
Explored and cleaned the client and price datasets, analyzing consumption, contract, and pricing data in Python to surface early patterns related to churn and prepare the data for feature engineering.

### 📂 [Task 4 – Feature Engineering](./Task%204)
Engineered new features to test the price-sensitivity hypothesis more directly — including price differences across peak/off-peak periods and month-over-month price variation — alongside date decomposition, categorical encoding, skew correction, and correlation-based feature pruning to prepare a clean modeling dataset.

### 📂 [Task 5 – Predictive Modeling](./Task%205)
Built and evaluated a Random Forest classification model to predict customer churn, using accuracy, precision, and recall. Analyzed feature importance to identify the true drivers of churn — finding that net margin and consumption behavior mattered more than the engineered price-sensitivity features.

### 📂 [Task 6 – Insights and Recommendations](./Task%206)
Synthesized the findings from the full analysis into a single-slide executive summary for senior stakeholders, following the SCQA (Situation–Complication–Question–Answer) framework to communicate the business recommendation clearly and concisely.

---

## Key Takeaways

- Price sensitivity is **not** the primary driver of churn for PowerCo's SME customers.
- Net margin and 12-month consumption emerged as stronger predictors of churn than any price-based feature.
- Recommendation: shift retention strategy away from blanket price discounts, toward a targeted, model-driven approach focused on high-risk customers.

---

## About Forage

Forage virtual job simulations provide hands-on experience by replicating real workplace tasks from leading companies. They help learners develop practical skills through self-paced, project-based learning.

---

## Acknowledgements

- BCG X
- Forage

---

*This repository is intended for educational and portfolio purposes to showcase the work completed during the BCG X Data Science Virtual Job Simulation.*
