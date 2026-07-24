## 🎯 Task 6: Insights & Recommendations

## Overview

This project was completed as part of the **BCG X Data Science Job Simulation** on **Forage**.

The objective was to synthesize the findings from the full analysis — business framing, EDA, feature engineering, and modeling — into a single-slide executive summary for PowerCo's senior stakeholders, following the **SCQA (Situation–Complication–Question–Answer)** framework.

---

## Business Scenario

With the churn model built and evaluated, the final step was to step back from the technical work and communicate what it actually meant for PowerCo's business. Senior stakeholders don't need the modeling details — they need a clear, top-down summary of the problem, the finding, and the recommended next step, on a single slide.

---

## The SCQA Framework

A good executive summary provides all the key information in one slide. Consultants typically communicate "top down," starting with the conclusion and then providing supporting detail — the goal is to convey as much information in as few words as possible.

- **Situation** — summarize the background, before any findings
- **Complication** — identify the problem or opportunity that emerged
- **Question** — state the hypothesis or question that follows from the complication
- **Answer** — propose a solution and its potential impact

---

## Approach

### 1. Revisit the Full Case

Reviewed the findings from every prior task — the original price-sensitivity hypothesis (Task 2), the churn rate and early patterns from EDA (Task 3), the engineered price-variation features (Task 4), and the model's performance and feature importance results (Task 5) — to identify what actually mattered for the final recommendation.

### 2. Structure the Narrative with SCQA

**Situation** — background, no findings yet
- PowerCo, an energy retailer, asked BCG to investigate whether price sensitivity is driving customer churn, given a churn rate of ~9.7% across ~14,600 SME customers
- A Random Forest model was built on consumption, pricing, and contract data to test this hypothesis and flag customers likely to churn

**Complication** — the tension/problem, still no resolution stated
- Churn erodes revenue directly, and retention is cheaper than new customer acquisition, so getting the driver right matters
- The analysis shows price sensitivity is **not** the main driver; net margin and consumption behavior matter more — challenging the original assumption that discounting is the fix

**Question**
- Given that price isn't the main lever, how should PowerCo target retention spend, and should broad discounting continue at all?

**Answer**
- Move away from blanket discounts; use the model's risk scores to prioritize outreach to high-value, high-risk customers, and refine the model further before rolling out a full targeting program

### 3. Design for a Single Slide

Built the summary onto a single, clean slide using PowerCo's executive summary template — leading with the recommendation, using short, scannable bullets, and keeping supporting detail to the minimum needed to justify the conclusion.

---

## Key Skills Demonstrated

- Executive-level business communication
- Structuring an argument using the SCQA / pyramid principle
- Synthesizing multi-stage technical analysis into a single, decision-ready recommendation
- Slide design for a senior, non-technical audience

---

## Deliverables

- [`Executive_Summary_Answer.pdf`](./Executive_Summary_Answer.pdf) — completed executive summary slide
- [`Executive_Summary_Best_Practices.pdf`](./Executive_Summary_Best_Practices.pdf) — SCQA framework reference
- [`Executive_Summary_Template.pptx`](./Executive_Summary_Template.pptx) — editable slide template

---

## Learning Outcomes

Through this task, I gained hands-on experience with:

- Distilling a multi-stage data science project into a single, decision-ready slide
- Structuring a recommendation using the SCQA / pyramid principle used across management consulting
- Leading with the "so what" rather than the methodology, for a senior audience
- Translating a model's technical findings (feature importance, low recall) into plain-language business implications
