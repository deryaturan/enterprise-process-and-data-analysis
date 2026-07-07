# Enterprise Process and Data Analysis: Telecom Churn Project

This repository contains an end-to-end data analytics and business process optimization project. The objective is to analyze telecom customer churn data, identify high-risk high-value sub-segments, and design an operational workflow to maximize customer retention.

The project bridges the gap between raw data engineering and corporate operations by delivering both technical analysis and business process maps.

---

## Repository Structure

The project is organized into three dedicated phases to demonstrate structured documentation and separation of concerns:

```text
enterprise-process-and-data-analysis/
│
├── 1-data-and-analysis/
│   ├── telecom_churn_data.csv         # Raw customer dataset (7,043 rows)
│   ├── business_analysis.ipynb        # Data cleaning, EDA, and filtering script
│   └── actionable_risk_customers.csv  # Output list of 454 high-risk VIP customers
│
├── 2-process-design/
│   └── customer_retention_process.md  # Operational retention workflow (Mermaid Flowchart)
│
└── 3-project-management/
    └── project_management_summary.md  # Project phases and personal retrospective

```

---

## Phase Breakdown

### 1. Data and Analysis

The analysis was performed using Python (Pandas, Seaborn, Matplotlib) on a dataset containing 7,043 telecom customers.

* **Data Cleaning:** Transformed the TotalCharges column from string format to numeric, dropping missing values introduced by new customers with 0 tenure.
* **Exploratory Data Analysis (EDA):** Analyzed the churn correlation with key services. Identified that customers without Tech Support and those on Month-to-month contracts have the highest churn rates.
* **Targeted Filtering:** Isolated high-value customers who pay above-average monthly rates (MonthlyCharges > 64.76) but are on short-term contracts with low tenure (less than or equal to 18 months). This resulted in an actionable list of 454 VIP high-risk customers exported to a standalone CSV.

### 2. Process Design

Instead of leaving the data as a static report, an operational strategy was designed to save the identified customers:

* **Workflow Automation:** Drafted a Top-Down process flowchart using Mermaid notation to integrate Python outputs directly into the company's CRM system.
* **Retention Strategy:** Modeled a 48-hour SLA intervention loop where dedicated customer service agents offer a 15% discount tied to a 1-Year Contract.
* **KPI Alignment:** Defined standard corporate metrics to evaluate operational success (Retention Success Rate, SLA Compliance, and Saved Monthly Recurring Revenue).

### 3. Project Management

The repository was executed following a strict personal product management framework:

* Tasks were clearly divided into data engine engineering and business value mapping phases.
* Documented a personal retrospective identifying current architectural limitations and outlining future improvements, such as migrating from hardcoded thresholds to predictive Machine Learning models.

---

## Technical Stack and Tools

* **Language:** Python
* **Libraries:** Pandas, Matplotlib, Seaborn
* **Environment:** VS Code / Jupyter Notebooks
* **Notation:** Mermaid / Business Process Model and Notation (BPMN) principles