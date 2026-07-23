## 📧 Task 2: Problem Framing & Hypothesis

## Overview

This project was completed as part of the **BCG X Data Science Job Simulation** on **Forage**.

The objective was to frame PowerCo's customer churn problem as a testable hypothesis, identify the data required to investigate it, and outline a structured analytical approach — communicated as an email to the senior data scientist on the case.

---

## Business Scenario

**PowerCo**, a major gas and electricity utility supplying small and medium-sized enterprises (SMEs), is concerned about customer **churn** in an increasingly competitive energy market. The Associate Director's working hypothesis is that customers have become more **price sensitive** and are switching to lower-cost providers.

Working alongside senior data scientist Estelle Altazin, the task was to determine:

1. What data would be needed to investigate the drivers of customer churn?
2. What analytical steps and techniques would be used to test whether price sensitivity is the cause?

---

## Approach

### 1. Data Requirements

Identified the customer-level data needed to test the price-sensitivity hypothesis:
- Historical electricity and gas prices, and billing information
- Contract type and duration
- Energy consumption
- Customer tenure
- Churn status
- Customer service interactions
- Payment history
- Location and relevant demographic or business information
- Competitor pricing data (if available), for market context

### 2. Analytical Approach

Outlined a structured plan following BCG X's 5-step data science methodology:

1. **Exploratory data analysis & data cleaning** — understand the dataset, address missing values, and identify trends or anomalies
2. **Feature engineering** — create variables such as price sensitivity, usage patterns, and customer tenure
3. **Modeling** — build and compare binary classification models (Logistic Regression, Decision Tree, Random Forest) to predict churn
4. **Evaluation** — assess model performance using Accuracy, Precision, Recall, F1-score, and ROC-AUC
5. **Insights** — use feature importance analysis to quantify the impact of price sensitivity relative to other factors

### 3. Communication

Summarized the data requirements and proposed approach in an email to Estelle, to align the team before starting hands-on analysis.

---

## Deliverable

**Subject:** Approach to Investigating Customer Churn at PowerCo

> Hi Estelle,
>
> Following our discussion on the PowerCo case, I have outlined the data requirements and the analytical approach I propose for investigating the drivers of customer churn.
>
> To assess whether price sensitivity is a key factor influencing churn, we should request customer-level data including historical electricity and gas prices, billing information, contract type and duration, energy consumption, customer tenure, churn status, customer service interactions, payment history, location, and relevant demographic or business information. If available, competitor pricing data would also provide valuable market context.
>
> Once the data is available, I will follow a structured data science approach. I will begin with exploratory data analysis (EDA) and data cleaning to understand the dataset, address missing values, and identify trends or anomalies. Next, I will perform feature engineering by creating variables such as price sensitivity, usage patterns, and customer tenure. To test the hypothesis, I will build and compare binary classification models, such as Logistic Regression, Decision Trees, and Random Forest, to predict customer churn. Model performance will be evaluated using metrics including Accuracy, Precision, Recall, F1-score, and ROC-AUC, and feature importance analysis will be used to quantify the impact of price sensitivity relative to other factors.
>
> The insights from this analysis will help determine whether price sensitivity is the primary driver of churn or whether other customer or market factors have a greater influence, enabling us to provide actionable recommendations to improve customer retention.
>
> Kind regards,
> Simerjeet Kaur
> Junior Data Scientist

Full email: [`Task2_Email.pdf`](./Task2_Email.pdf)

---

## Key Skills Demonstrated

- Hypothesis formulation
- Data requirements scoping
- Structuring an end-to-end analytics approach
- Stakeholder communication

---

## Learning Outcomes

Through this task, I gained hands-on experience with:

- Translating a business concern (churn) into a testable data science hypothesis
- Identifying the right data points needed to validate or disprove a hypothesis
- Structuring a multi-step analytical plan before touching any data
- Communicating a technical plan clearly and concisely to a senior stakeholder
