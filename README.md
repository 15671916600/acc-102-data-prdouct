# SportBrands_FinancialAnalysis: Nike vs Adidas Financial Performance Comparison (2021-2025)
**ACC102 Track 2 - GitHub Data Product | XJTLU IBSS**

> 🎥 Demo Video Link: <替换成你的1-3分钟演示视频链接>
> 
> **Repository Topics**: `xjtlu` `acc102` `python` `data-analysis` `financial-analysis` `nike` `adidas`

---

## 📋 Table of Contents
1.  [1. Project Overview](#1-project-overview)
2.  [2. Dataset Information](#2-dataset-information)
3.  [3. Python Analytical Workflow & Methods](#3-python-analytical-workflow--methods)
4.  [4. Key Findings & Insights](#4-key-findings--insights)
5.  [5. Repository Structure](#5-repository-structure)
6.  [6. How to Reproduce the Analysis](#6-how-to-reproduce-the-analysis)
7.  [7. Limitations & Future Improvements](#7-limitations--future-improvements)
8.  [8. AI Use Disclosure](#8-ai-use-disclosure)

---

## 1. Project Overview
This project conducts a comprehensive, data-driven comparison of the financial performance of two global sportswear market leaders, **Nike Inc.** and **Adidas AG**, over the 2021 to 2025 fiscal years. The analysis focuses on three core financial metrics that reflect business scale, profitability, and shareholder return: **annual Revenue**, **Earnings Per Share (EPS)**, and **Return on Equity (ROE)**.

### Analytical Problem
This project addresses three core business questions aligned with business and financial analysis requirements:
1.  What are the differences in revenue scale, growth momentum, and operational stability between Nike and Adidas in the post-pandemic period (2021-2025)?
2.  How do the two brands differ in profitability stability and per-share earnings performance for investors?
3.  Which company delivers more consistent and higher returns for its shareholders, as measured by annualized Return on Equity (ROE)?

### Target Audience
This project is designed for the intended users defined in the assignment:
- Entry-level investment analysts and retail investors evaluating sportswear sector investment opportunities
- Undergraduate business/accounting/finance students learning financial statement analysis and Python-based data analytics
- Sportswear industry researchers seeking a clear, data-backed overview of the two market leaders' 5-year financial performance

---

## 2. Dataset Information

| Item | Full Official Details |
|------|------------------------|
| **Primary Data Source** | Official audited annual financial reports from Nike Inc. and Adidas AG (2021-2025 full fiscal years) |
| **Official Source Links** | [Nike Investor Relations Official Website](https://investors.nike.com/) <br> [Adidas Group Investor Relations Official Website](https://www.adidas-group.com/en/investors/) |
| **Data Access Date** | 24th April 2026 |
| **Data Storage Location** | All cleaned, structured data files are stored in the `SportBrands_FinancialAnalysis/data/` directory of this repository |
| **Core Metrics Definition** | • `Revenue`: Annual total operating revenue, denominated in **Million USD** <br> • `EPS`: Annual basic earnings per share, denominated in **USD** <br> • `ROE`: Annualized return on shareholder equity, presented as a **percentage (%)** |
| **Data Quality Validation** | The dataset has been fully cleaned and validated, with 0 missing values across all metrics and fiscal years for both companies |

---

## 3. Python Analytical Workflow & Methods
All data processing, analysis, and visualization are completed using Python, with a fully reproducible end-to-end workflow that meets the assignment's substantive Python work requirements.

### Core Python Libraries Used
- `pandas`: Data loading, column name standardization, time range filtering, missing value validation, year-on-year growth rate calculation, and cross-company dataset merging
- `matplotlib` & `seaborn`: Professional standardized data visualization, including line charts for long-term trend analysis and grouped bar charts for annual side-by-side performance comparison
- `openpyxl`: Excel file reading and structured data import
- `numpy`: Numeric operations for visualization layout and data processing

### Full End-to-End Analytical Workflow
1.  **Library Import & Environment Setup**: Import all required dependencies and set consistent, professional visualization styles for all outputs
2.  **Data Loading**: Import cleaned annual financial datasets for Nike and Adidas from the `SportBrands_FinancialAnalysis/data/` directory
3.  **Data Preprocessing & Quality Control**:
    - Standardize column names for consistent cross-company comparison
    - Filter data to retain only the 2021-2025 fiscal year range as defined in the project scope
    - Validate data quality by checking and reporting missing values for all metrics
4.  **Derivative Metric Calculation**: Compute year-on-year revenue growth rates (%) for both companies to evaluate and compare growth momentum
5.  **Dataset Merging**: Combine Nike and Adidas datasets into a single structured dataframe for unified visualization and comparative analysis
6.  **Data Visualization & Output**:
    - Line chart: 5-year annual revenue trend comparison between the two brands
    - Grouped bar chart: Annual EPS side-by-side comparison for each fiscal year
    - Line chart: 5-year ROE trend and stability comparison for shareholder return analysis
7.  **Descriptive Statistical Summary**: Calculate 5-year average values for all three core metrics to summarize long-term performance differences between Nike and Adidas

---

## 4. Key Findings & Insights
All findings are directly derived from the quantitative Python analysis of the 2021-2025 dataset, fully aligned with the project's analytical problem:
1.  **Revenue Scale & Growth Performance**: Nike maintained a dominant revenue lead across all 5 years, with an average annual revenue of **48,027.2 Million USD** – nearly double Adidas' average annual revenue of **24,934.0 Million USD**. Nike delivered consistent positive growth in 2022-2024, while Adidas experienced revenue declines in 2022 and 2023 before returning to stable growth in 2024-2025.
2.  **EPS Stability & Profitability Consistency**: Nike's EPS remained consistently positive and stable between 2.16-3.75 USD throughout the 5-year period. In contrast, Adidas' EPS saw extreme volatility, including a **negative EPS of -0.73 USD in 2023** due to operational and inventory challenges, highlighting significantly weaker profitability stability compared to Nike.
3.  **Shareholder Return Efficiency (ROE)**: Nike delivered substantially higher and more stable ROE, with a 5-year average of **36.38%**, more than double Adidas' average ROE of **15.20%**. Even at its lowest point in 2025 (20.2%), Nike's ROE remained competitive with Adidas' peak 2021 value (28.1%), reflecting consistently stronger profitability efficiency for Nike's shareholders.
4.  **Post-Downturn Recovery Trend**: Adidas showed clear signs of operational and financial recovery in 2024-2025, with rebounding revenue growth, positive and rising EPS, and a sharp increase in ROE, narrowing the performance gap with Nike after its 2022-2023 operational downturn.

---

## 5. Repository Structure
This section defines the exact file structure of this GitHub repository, so markers can easily navigate all files:
Root/
├── README.md
├── financial_analysis.ipynb
├── requirements.txt
└── SportBrands_FinancialAnalysis/
└── data/
├── nike_financials.xlsx
└── adidas_financials.xlsx
