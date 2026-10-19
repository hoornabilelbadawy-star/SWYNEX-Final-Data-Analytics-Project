# Swynex Internship — Customer Personality Analysis

## Project Overview
This project explores customer personality and purchasing behavior as part of my internship with Swynex. The workflow covers data cleaning, exploratory data analysis, reporting, and an interactive Excel dashboard.

## Problem Statement
The business needs a clearer view of customer characteristics, product spending, purchasing channels, and campaign responses. The analysis aims to organize the customer data, identify useful patterns, and translate findings into practical questions and recommendations for business decisions.

## Dataset Information
- **Dataset:** Customer Personality Analysis
- **Source:** [Kaggle — Customer Personality Analysis](https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis)
- **Grain:** One row represents one customer.
- **Tools:** Excel Power Query, SQL Server Management Studio (SQL), Excel charts/dashboard, GitHub.

> The dataset contains customer demographics, income, product spending, purchase-channel activity, deal purchases, and campaign-response fields. Check the final workbook before publishing exact figures.

## 1. Data Cleaning and Preparation
Completed in Excel Power Query:
- Checked customer IDs for duplicate records.
- Trimmed leading/trailing spaces in categorical fields such as Education and Marital_Status.
- Flagged unexpected Marital_Status values (including `Absurd` and `YOLO`) for review rather than silently changing the original values.
- Reviewed missing Income values and income outliers; retained the original Income field and created a cleaned field with missing values filled using the median.
- Parsed enrollment dates stored as text using the appropriate day-month-year locale.
- Reviewed campaign fields and distinguished campaign response from complaint-related fields.
- Reviewed columns with only one distinct value for usefulness in analysis.

## 2. Exploratory Data Analysis
SQL was used to explore the cleaned data, followed by Excel charts and a mini-report.

Analysis areas:
- Overall customer and income/spending metrics.
- Customer spending by marital status and education.
- Age-group comparisons.
- Spending across wine, fruit, meat, fish, sweets, and gold products.
- Purchase activity by web, catalog, and store channels.
- Campaign acceptance versus decline.
- Spending behavior across income segments.

**Metric note:** `NumDealsPurchases` represents purchases made using deals, not total orders. Channel purchase counts should not be described as revenue. Confirm final KPI values against the workbook before sharing.

## 3. Interactive Dashboard
The completed Excel dashboard includes KPI cards for:
- Customer Total Spend
- Number of Purchases
- Average Recency
- Average Income
- Average Spend per Person
- Channel Purchases

It also includes filters for campaigns 2–5 and visuals covering:
- Contribution by marital status and education
- Age distribution
- Total spend
- Sales by product
- Sales by channel
- Campaign performance
- Income versus spending

A dashboard walkthrough video was recorded separately.

## Key Business Insights
The analysis highlighted several patterns to investigate further:
1. Product categories contribute differently to overall spending; wine was the leading category in the analysis.
2. Store purchases were the most frequent channel, followed by catalog and web purchases.
3. Campaign declines substantially outnumbered acceptances, suggesting that campaign targeting and offer relevance deserve review.
4. Customer groups differ in total contribution and average spending; segment size and average spend should be considered together.
5. Income and spending do not necessarily move in a simple one-to-one pattern, so customer segmentation should consider purchasing behavior as well as income.

These are descriptive findings, not proof of causation. Exact values and category rankings should be verified against the final workbook before publication.

## Recommendations
- Compare campaign acceptance rates, not just raw acceptance/decline counts.
- Test customer segments and offers to understand which audiences respond best.
- Track both total spend and average spend when comparing demographic groups.
- Review product-category and channel performance together before making allocation decisions.
- Keep a documented, repeatable cleaning process for future updates.

## Challenges and Learning
- Identifying unexpected category values without losing the original data.
- Handling missing income values while reviewing outliers.
- Correctly parsing text dates.
- Distinguishing campaign response from complaint fields.
- Understanding the difference between deal purchases, channel purchase counts, and total orders.
- Moving from SQL-based exploration to Excel reporting and an interactive dashboard.

## Deliverables
- `Swynex_Customer_Personality_Analysis_Project_Report.pdf` — detailed project report.
- Final Excel workbook — cleaned data, analysis, charts, and interactive dashboard (add this file to the repository).
- Dashboard walkthrough video (optional; add a link or upload if appropriate).

## Suggested Repository Structure
```text
customer-personality-analysis/
├── README.md
├── Swynex_Customer_Personality_Analysis_Project_Report.pdf
├── data/
│   └── README.md
├── sql/
│   └── analysis_queries.sql
├── excel/
│   └── customer_personality_analysis.xlsx
└── dashboard/
    └── dashboard_walkthrough_link.txt
```

Only add files that are actually available. Do not upload sensitive data; check the dataset's terms and repository requirements before redistributing the raw dataset.

## Dataset Credit
Customer Personality Analysis dataset by Imakash3011 on Kaggle: https://www.kaggle.com/datasets/imakash3011/customer-personality-analysis

## Project Status
The three project tasks—data preparation, exploratory analysis, and interactive dashboard—have been completed. Before final submission, verify exact figures in the final workbook and ensure the workbook/report are accessible from the public repository.
