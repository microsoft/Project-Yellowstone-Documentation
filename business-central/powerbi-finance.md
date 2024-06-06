---
title: Power BI reports on finance data
description: Learn how to use the Power BI reports to analyze finance data.
author: kennienp
ms.author: kepontop
ms.reviewer: bholtorf
ms.topic: conceptual
ms.search.keywords: bi, power BI, analysis, KPI
# ms.search.form: 516, 9300, 5119, 9301, 9305
ms.date: 05/28/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Power BI reports on finance data

This article explains how to use the built-in **Power BI reports** to analyze finance data. You don't have to run a report or switch to another application, such as Excel. The feature provides an interactive and versatile way to calculate, summarize, and examine data in curated reports with pre-defined KPIs. 

The Power BI reports on finance data supports many analytics scenarios relevant for finance processes, such as

- Scenario 2 
- Scenario 10 
- Scenario 12


## Available KPIs for finance

The following sections provide an overview of all the available KPIs that are shown on the Power BI reports for finance:

| KPI | Usage example | Available on Report | Learn more |
| --- | ------------- | ------------------- | ---------- |
| KPI 1 | TODO | Finance overview | [Finance overview Report](#finance-overview-report) |
| KPI 2 | TODO | Finance overview | [Finance overview Report](#finance-overview-report) |


## Available Power BI reports for finance

The following sections provide an overview of all the available Power BI reports for finance:

| Report | Usage examples | Learn more |
| ------ | -------------- | ---------- |
| Finance overview | TODO | [Finance overview Report](#finance-overview-report) |
| Liquidity KPIs | TODO | [Liquidity KPIs Report](#liquidity-kpis-report) |


### Finance overview Report

The _Financial overview_ is designed to provide a comprehensive snapshot of an organization's financial health and performance. This dashboard displays key financial metrics (KPIs) to give stakeholders a clear view of revenue, cost management, profitability, and financial stability. The Finance overview is typically used in the following scenarios:

- Executive Decision-Making: Helping executives and senior management make informed strategic decisions by providing a high-level view of the financial status.
- Financial Analysis: Supports financial analysts in assessing trends, identifying anomalies, and making data-driven recommendations for improvements.
- Operational Monitoring: Assists operational managers in monitoring financial performance against targets and budgets to ensure operational efficiency and effectiveness.

![Screenshot of the Finance overview report](./media/finance-powerbi-finance-overview.png "Finance Overview (screenshot)")

The report shows the following KPIs:

- Revenue
- Expenses
- Gross Profit
- Gross Profit Margin
- Net Profit
- Net Profit Margin
- Liabilities
- Assets
- Debt Ratio
- Operating Profit- EBIT
- EBITDA (Earnings Before Interest, Taxes, Depreciation, and Amortization)
- Operating Expenses
- Balance (AP)
- Balance (AR)
- Cost of Goods Sold across time
- Net Profit across time

#### Revenue (also known as Gross Revenue)

**KPI description**

Revenue is the amount of money that a company receives from its customers for the products or services it sells. It is also called gross revenue, sales, or income. Revenue is the top line of the income statement and reflects the total value of transactions with customers before deducting any expenses, such as the cost of goods sold (COGS), operating expenses, taxes, or interest. 

**Usage scenario(s)**

You can use revenue to measure the overall performance and growth of your business, as well as the effectiveness of your sales and marketing strategies. Revenue indicates the demand and value of your products or services in the market, as well as your ability to attract and retain customers.

- **Business Segment Profitability:** By analyzing Revenue by different business segments (dimensions), companies can identify which areas are contributing the most to the top line and adjust their focus and resources accordingly.
- **Financial Planning:** Revenue recognition is crucial for financial planning, forecasting, and budgeting, helping businesses to make informed decisions about future investments and expenses.
- **Sales Team Evaluation:** Analyzing Revenue KPI can help in evaluating the performance of sales teams, understanding the effectiveness of sales strategies, and identifying areas for improvement.

**Calculation**

Revenue is calculated as follows: The Net Change for all accounts categorized by the Revenue (Level 1 Category) parameter.

**Data source(s)**

To calcuate Revenue, data from the following tables is used: 
- G/L Entries
- G/L Account Category
- Revenue (Level 1 Category)


### Gross Profit Margin

**KPI description**

KPI 1 is...

**Usage scenario(s)**

You use KPI 1 to...

**Calculation**

KPI 1 is calculated as follows: ...

**Data source(s)**

To calcuate KPI 1, data from the following tables is used: _table 1_, _table 2_, and _table 3_...


## Data foundation for the Power BI reports on finance

The Power BI reports on finance is based on the following tables in Business Central:

- Table 1
- Table 2


<!-- ## See also -->

