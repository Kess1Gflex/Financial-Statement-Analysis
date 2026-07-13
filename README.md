# Financial Statement Analysis using Python

A financial data analysis project that evaluates company profitability, operational performance, customer contribution, supplier costs, and financial trends using Python, Pandas, and Matplotlib.

---

# Project Context

Financial statement analysis helps organizations evaluate their financial health by measuring profitability, liquidity, and operational performance. This project analyzes a transactional financial dataset to uncover the factors driving the company's financial performance and provide data-driven recommendations for improving profitability.

---

# Problem Statement

The company has experienced declining profitability across multiple departments and reporting periods. Management requires a data-driven assessment to understand the key drivers behind this performance and identify opportunities for improvement.

This project answers the following business questions:

- Which departments contribute the most to profitability?
- How has gross profitability changed over time?
- Are all branches performing equally, or are some branches outperforming others?
- Who are the company's most valuable customers based on revenue contribution?
- How is procurement spending distributed across vendors?

---

# Dataset Overview

| Attribute | Value |
|-----------|------:|
| Total Records | 800 |
| Total Features | 14 |
| Dataset Type | Financial Transactions |
| Reporting Period | January 2025 – June 2026 |

### Key Variables

- Transaction ID
- Date
- Department
- Branch
- Customer
- Vendor
- Revenue
- Cost of Goods Sold (COGS)
- Operating Expense
- Assets
- Liabilities
- Equity
- Status

---

# Data Cleaning

The dataset was inspected and cleaned before analysis to improve data quality while preserving the integrity of the original financial records.

Cleaning activities included:

- Standardizing inconsistent department names
- Standardizing vendor names
- Standardizing branch names
- Standardizing payment status values
- Removing leading and trailing whitespace
- Converting date values to datetime format
- Investigating duplicate transaction IDs
- Validating missing values
- Preserving missing financial values where there was insufficient business justification for imputation

---

# Feature Engineering

To support the financial analysis, the following financial metrics were created:

- Gross Profit
- Gross Margin
- Operating Profit
- Operating Margin
- Working Capital
- Current Ratio
- Debt-to-Equity Ratio

---

# Business Questions & Insights

## 1. Which departments contribute the most to profitability?

![Gross Profit by Department](images/Gross_Profit_by_Department.png)

### Findings

- Every department recorded a negative Gross Profit.
- Sales generated the largest gross loss.
- Finance recorded the smallest gross loss.
- Revenue remained consistently lower than Cost of Goods Sold across every department, indicating that the profitability challenge is company-wide rather than department-specific.

---

## 2. How has gross profitability changed over time?

![Gross Profit Trend](images/Trend_in_Gross_Profitability.png)

### Findings

- Gross Profit remained negative for most of the reporting period.
- The first major profitability decline occurred in August 2025.
- The deepest losses were recorded in October and December 2025, followed by another significant decline in March 2026.
- Profitability gradually recovered between May and June 2026.

---

## 3. Are all branches performing equally, or are some branches outperforming others?

![Branch Performance](images/Branch_Gross_Loss.png)

### Findings

- Branches contributed differently to the company's overall gross losses.
- The analysis identified which branches accounted for the largest share of company-wide losses, providing management with areas requiring operational review.

---

## 4. Who are the company's most valuable customers based on revenue contribution?

![Customer Revenue Distribution](images/Customer_Revenue_Distribution.png)

### Findings

- Revenue is relatively evenly distributed across the company's three customers.
- No single customer dominates total revenue.
- However, relying on only three customers creates customer concentration risk.

---

## 5. How is procurement spending distributed across vendors?

![Vendor Supply Cost](images/Vendor_Supply_Cost.png)

### Findings

- Procurement spending is relatively balanced between Vendor A and Vendor B.
- The company does not appear to rely heavily on a single supplier, reducing supplier concentration risk.

---

# Business Recommendations

Based on the analysis, the following recommendations are proposed:

- Review procurement strategies and supplier contracts to reduce Cost of Goods Sold.
- Investigate the operational changes that occurred around August 2025 when profitability began to decline significantly.
- Expand the customer base to reduce dependence on only three customers.
- Continue monitoring branch performance to identify operational improvement opportunities.
- Track financial KPIs regularly to monitor profitability trends and support strategic decision-making.

---

# Technologies Used

- Python
- Pandas
- Matplotlib
- Jupyter Notebook
- Git
- GitHub
