---
title: Finance Overview Report
description: 
author: johnathan gonzalez
ms.author: kepontop
ms.reviewer: 
ms.topic: conceptual
ms.search.keywords: bi, power BI, analysis, KPI
# ms.search.form: 516, 9300, 5119, 9301, 9305
ms.date: 05/28/2024
ms.service: dynamics-365-business-central
ms.custom: bap-template
---

# Finance Overview Report

## Overview

The *Financial Overview* report is designed to provide a high-level snapshot of an organization's financial health and performance. This dashboard displays key financial metrics (KPIs) to give stakeholders a clear view of revenue, cost management, profitability, and financial stability. 

The finance overview is typically used in the following scenarios:

- Executive Decision-Making: Helping executives and senior management make informed strategic decisions by providing a high-level view of the financial status.
- Financial Analysis: Supports financial analysts in assessing trends, identifying anomalies, and making data-driven recommendations for improvements.
- Operational Monitoring: Assists operational managers in monitoring financial performance against targets and budgets to ensure operational efficiency and effectiveness.

:::image type="content" source="media/finance/financial-overview.png" alt-text="Screenshot of the Finance Overview report" lightbox="media/finance/financial-overview.png":::

## KPIs on the Financial Overview Report

- [Revenue](#revenue)
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
- [Balance (AP)](#balance-ap)
- Balance (AR)
- Cost of Goods Sold across time
- Net Profit across time
 
### Revenue

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

To calculate Revenue, data from the following tables is used: 
- G/L Entries
- G/L Account Category
- **Parameter**: Revenue (Level 1 Category)


### Gross Profit Margin

**KPI description**

Gross Profit Margin is a financial metric that indicates the percentage of revenue remaining after deducting the cost of goods sold (COGS). It is calculated by subtracting COGS from revenue and expressing the result as a percentage of revenue. This metric is essential for understanding a company's profitability before accounting for other expenses like selling, general, and administrative costs.

**Usage scenario(s)**

- **Performance Benchmarking:** Gross Profit Margin can be used to benchmark performance against competitors. This helps in understanding competitive positioning and identifying areas where the company can improve its cost structure or pricing strategies to match or exceed industry standards.
- **Evaluating Cost Efficiency:** To assess how well a company manages its cost of goods sold relative to its revenue. By analyzing Gross Profit Margin, businesses can identify inefficiencies in their production processes or supply chains and take measures to reduce costs, thereby improving profitability.
- **Pricing Strategy Assessment:** To determine the effectiveness of current pricing strategies businesses can compare Gross Profit Margin across different dimensions such as product lines or services. A low margin might indicate the need for a price increase or cost reduction, while a high margin might suggest pricing power or the potential to lower prices to gain market share.

**Calculation**

Gross Profit Margin is calculated as follows: Gross Profit divided by Revenue, expressed as a percentage. 

**Data source(s)**

To calculate Gross Profit Margin, data from the following tables is used: 
- G/L Entries
- G/L Account Category
- **Parameter**: Revenue (Level 1 Category)
- **Parameter**: Cost of Goods Sole (Level 1 Category)

### Balance (AP)

**KPI description**

Balance (AP) also known as Accounts Payable Balance is a metric that represents the total amount of a company's outstanding payables. By tracking the Balance of Aged Payables, businesses can manage cash flow, maintain supplier relationships, and ensure timely payments to avoid late fees and interest charges. 

**Usage scenario(s)**
- **Financial health assessment**: To assess the company’s financial obligations and stability. A high Accounts Payables Balance, especially with many overdue invoices, can indicate cash flow problems or poor financial management. Conversely, a well-managed payables balance can indicate strong financial health and prudent cash management practices.
- **Risk management**: Monitoring the Aged Payables Balance helps businesses avoid penalties and interest on overdue invoices, reducing the risk of damaging credit ratings or supplier relationships.

**Calculation**

Balance (AP) is calculated as follows: The measure is calculating the [Amount Payable (LCY)] up to and including the maximum date in the Date filter context.

**Data source(s)**

To calculate Balance (AP), data from the following tables is used: 
- Vendor Ledger Entries
- Date 

### EBITDA

**KPI description**
EBITDA stands for Earnings Before Interest, Taxes, Depreciation, and Amortization. It provides insight into a company's core profitability by focusing on earnings generated from 

**Usage scenario(s)**
- PLACEHOLDER
- PLACEHOLDER

**Calculation**

PLACEHOLDER

**Data source(s)**

PLACEHOLDER

## Data foundation for the Power BI reports on finance

The Power BI reports on finance is based on the following tables in Business Central:

- Table 1
- Table 2


<!-- ## See also -->

