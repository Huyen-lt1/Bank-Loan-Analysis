# Bank-Loan-Analysis
Financial Loan Analysis and Portfolio Quality Assessment using Python.
#  Bank Loan Analysis & Financial Portfolio Assessment

![Python](https://img.shields.io/badge/Python-3.8%2B-blue?style=flat&logo=python)
![Pandas](https://img.shields.io/badge/Pandas-Data%20Analysis-150458?style=flat&logo=pandas)
![Status](https://img.shields.io/badge/Status-Completed-success)

##  Executive Summary
This project presents an end-to-end Exploratory Data Analysis (EDA) on bank financial loans. The main objective is to evaluate loan portfolio quality, track key performance indicators (KPIs) such as Month-to-Date (MTD) funded amounts and received payments, and analyze credit risk through **Good Loan vs. Bad Loan** categorization. 

The insights derived from this analysis help financial institutions optimize risk management strategies, reduce default rates, and balance loan approval rates.

---

## Key Business Metrics & Findings

### 1. Overall Portfolio Overview
* **Total Loan Applications:** `38,576`
* **MTD Loan Applications (Dec 2021):** `4,314`
* **Total Funded Amount:** `$435.76M`
* **MTD Total Funded Amount:** `$53.98M`
* **Total Amount Received:** `$435.76M`
* **MTD Total Amount Received:** `$58.07M`
* **Average Interest Rate:** `12.05%`
* **Average Debt-to-Income (DTI):** `13.33%`

### 2. Loan Quality Assessment (Risk Analysis)

| Category | Application Count | Share (%) | Funded Amount ($M) | Received Amount ($M) | Net Impact |
| :--- | :---: | :---: | :---: | :---: | :--- |
| **Good Loans** *(Fully Paid / Current)* | **33,243** | **86.18%** | **$370.22M** | **$435.79M** | +$65.57M Profit |
| **Bad Loans** *(Charged Off)* | **5,333** | **13.82%** | **$65.53M** | **$37.28M** | -$28.25M Loss |

> **Key Insight:** While 86.18% of the loans are performing well, the 13.82% default rate contributed to a direct loss of **$28.25M**. Mitigating default risks in high-risk sub-grades and high DTI segments is essential to boosting net profitability.

---

## Tech Stack & Libraries
* **Language:** Python 3.8+
* **Data Processing:** `pandas`, `numpy`
* **Data Visualization:** `matplotlib`, `seaborn`, `plotly`
* **Environment:** Jupyter Notebook / Google Colab

---

## Dataset Architecture
The dataset contains **38,576 rows** and **24 features** capturing borrower profiles and loan attributes:
* **Borrower Info:** `annual_income`, `dti`, `emp_length`, `emp_title`, `home_ownership`, `address_state`
* **Loan Info:** `loan_amount`, `term`, `int_rate`, `installment`, `grade`, `sub_grade`, `purpose`
* **Status & Dates:** `loan_status`, `issue_date`, `last_payment_date`, `total_payment`
