# Fetch Data Analyst Take-Home Assessment

## Overview
This repository contains my submission for the Fetch Data Analyst Take-Home Assessment. The project involves analyzing transactional, product, and user data to extract insights and provide recommendations based on the findings.

## Files in this Repository
- **Nikhil.ipynb** - The Jupyter Notebook containing my analysis, SQL queries, and insights.
- **data/** - Folder containing the provided CSV files (*USER_TAKEHOME.csv*, *TRANSACTION_TAKEHOME.csv*, *PRODUCTS_TAKEHOME.csv*).
- **README.md** - This file, providing an overview of the project.

## Approach
The analysis was conducted in three main parts:

### 1. Data Exploration
- Identified and resolved **data quality issues**, such as:
  - **Duplicate rows** in the Products (215) and Transactions (171) tables.
  - **Missing values** in CATEGORY_4 (92%) and LANGUAGE (30%) columns.
  - **Foreign key issues** where transactions lacked BARCODE values, making it hard to track product sales.
  - **Inconsistent formatting** (e.g., FINAL_QUANTITY containing text instead of numbers).

### 2. SQL Queries & Insights
- Extracted insights using SQL queries:
  - **Top 5 brands by receipts scanned** among users aged 21+.
  - **Top 5 brands by sales** among users who have had an account for 6+ months.
  - **Health & Wellness category sales** breakdown by generation.
  - Identified **power users** and leading brands in specific categories.

### 3. Stakeholder Communication
- Drafted a summary email highlighting:
  - **Key data issues and outstanding questions** for clarification.
  - **Interesting trends**, such as Millennials & Gen Z driving Health & Wellness sales.
  - **Recommendations & next steps** to clean up missing/duplicate data and refine further analysis.

## How to Run the Analysis
1. Clone this repository:
   ```bash
   git clone <repository-url>
   cd fetch-data-analyst-takehome
   ```
2. Install required Python packages:
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```
3. Open the Jupyter Notebook:
   ```bash
   jupyter notebook Nikhil.ipynb
   ```
4. Run the notebook cells to reproduce the analysis and insights.

## Next Steps
- Clarify **missing values in key columns** and whether to keep or remove them.
- Address **barcode inconsistencies** to improve transaction tracking.
- Standardize **data formats** for better accuracy in future analyses.
