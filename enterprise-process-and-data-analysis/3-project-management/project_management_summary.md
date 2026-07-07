# Project Planning and Task Breakdown

This document outlines how this repository was planned and executed as a self-managed portfolio project. Even as a solo developer, breaking the project into structured phases ensured organized delivery from data to process design.

---

## 1. Project Phases and Task Breakdown

Instead of writing code blindly, the project was organized into two main logical phases:

### Phase 1: Data Analytics and Risk Filtering (Backend Engine)
* **Goal:** Clean raw telecom data and filter actionable insights using Python.
* **Completed Tasks:**
    * Cleaned and formatted the TotalCharges column (handled empty spaces and type casting).
    * Created distribution and breakdown charts for InternetService and TechSupport.
    * Built statistical distributions (boxplots) to analyze high-paying, short-term contract users.
    * Isolated the exact 454 high-risk VIP customers into actionable_risk_customers.csv.

### Phase 2: Operational Mapping and Documentation (Business Value)
* **Goal:** Convert data insights into a real-world corporate strategy.
* **Completed Tasks:**
    * Designed an operational flowchart (customer_retention_process.md) explaining what the company should do with the 454 high-risk users.
    * Integrated a dynamic Mermaid flowchart to visualize the call-center retention workflow.
    * Defined measurable Business KPIs (Retention Success Rate, MRR Saved).

---

## 2. Personal Project Retrospective (Lessons Learned)

* **What Went Well:** The data filtering criteria successfully narrowed down 7,043 rows of messy data into a highly targeted list of 454 high-value customers, simulating how data drives actual business decisions.
* **Future Scope / Next Steps:** If I expand this project in the future, instead of using hardcoded rules for filtering (tenure <= 18), I plan to implement a Machine Learning model (like XGBoost or Logistic Regression) to predict the exact probability of customer churn.