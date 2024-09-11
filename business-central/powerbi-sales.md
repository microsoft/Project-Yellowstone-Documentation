---
title: Power BI reports on sales data
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

# Power BI reports on Sales Data

This article explains how to use the built-in **Power BI reports** to analyze finance data. You don't have to run a report or switch to another application, such as Excel. The feature provides an interactive and versatile way to calculate, summarize, and examine data in curated reports with pre-defined KPIs. 

The Power BI reports on finance data supports many analytics scenarios relevant for finance processes, such as

- Scenario 2 
- Scenario 10 
- Scenario 12


## Available KPIs for Sales

The following sections provide an overview of all the available KPIs that are shown on the Power BI reports for finance:

- [Sales KPIs](#sales-kpis)
- [Cost KPIs](#cost-kpis)
- [Gross Profit KPIs](#gross-profit-measures)
- [Sales Budget Measures](#sales-budget-measures)

#### Sales KPIs
| KPI | Usage example | Available on Report | Learn more | 
| --- | ------------- | ------------------- | ---------- |
| Sales Amount | - | - | TODO |
| Sales Quantity | - | - | TODO |
| No. of Distinct Items | A distinct count used to determine how many different items have been used across a given period.| N/A | TODO |
| No. of Outstanding Sales Orders | A distinct count used to determine the exact number of Sales Orders that have not been actioned. This is neither shipped or invoiced. |Sales Overview| TODO |
| No. of Posted Sales Invoices | A distinct count used to determine the exact number of posted sales invoices that have been fully processed. | Sales Overview | TODO |
| No. of Shipped Not Invoiced Sales Orders | A distinct count used to determine the exact number of Sales Orders that have been shipped not invoiced. |Sales Overview| TODO |



#### Cost KPIs
| KPI | Usage example | Available on Report | Learn more | 
| --- | ------------- | ------------------- | ---------- |
| Cost Amount | - | - | TODO |
| Cost Amount Non-Inv | - | - | TODO |


#### Gross Profit KPIs
| KPI | Usage example | Available on Report | Learn more | 
| --- | ------------- | ------------------- | ---------- |
| Gross Profit | - | - | TODO |
| Gross Profit Margin | - | - | TODO |


#### Sales Budget Measures
| KPI | Usage example | Available on Report | Learn more | 
| --- | ------------- | ------------------- | ---------- |
| Amount Receivable (LCY) | - | - | TODO |
| Balance (AR) | - | [Finance overview](#finance-overview-report) | TODO |
| Original Amount (LCY) | - | - | TODO |


## Available Power BI reports for sales

The following sections provide an overview of all the available Power BI reports for finance:

| Report | Usage examples | Learn more |
| ------ | -------------- | ---------- |
| Sales Overview | The Sales Overview can be used in executive decision-making, supporting order processing having a view of different order documents and key metrics on Salespeople and Customers. | [Sales Overview](#TODO) |
| Daily Sales | The Daily Sales report indicates the value of Sales across different days. This can be broken down into specific periods through drilling down. | [Daily Sales](#TODO) |
| Moving Average | TODO | [Moving Average](#TODO) |
| Moving Annual Total | TODO | [Moving Annual Total](#TODO) |
| Period-Over-Period Growth | TODO | [Period-Over-Period Growth](#TODO) |
| Month-To-Date | TODO | [Month-To-Date](#TODO) |
| Sales by Item | The Sales by Item report can be use to show how each customer is performing over a specific period. This can be used in conjunction with other reporting options. | [Sales by Item](#TODO) |
| Sales by Customer | The Sales by Customer report can be use to show how each customer is performing over a specific period. This can be used in conjunction with other reporting options. | [Sales by Customer](#TODO) |
| Sales by Salesperson | The Sales by Salesperson report can be use to show how each customer is performing over a specific period. This can be used in conjunction with other reporting options. | [Sales by Salesperson](#TODO) |
| Actual vs. Budget Quantity | The Actual vs Budget Quantity report can be used to make informed comparisons for sales reporting how sales quantity is going compared to the budget quantity. | [Actual vs. Budget Quantity](#TODO) |
| Actual vs. Budget Amount | The Actual vs Budget Amount report can be used to make informed comparisons for sales reporting how sales amount is going compared to the budget amount.  | [Actual vs. Budget Amount](#TODO) |


### Budget Amount

**Budget Amount description**

Budget Amount is a financial metric to indicate the amount for a specific budget based on your filtering.

**Usage scenario(s)**

You can use Budget Amount to highlight the specifc value of a specific budget and a period of time.

**Calculation**

Budget Amount is calculated as follows: The sum of Sales Amount from the Item Budget Entries.

**Data source(s)**

To calculate Budget Amount, data from the following tables is used: 
- Item Budget Entries

### Budget Amount Variance

**Budget Amount Varaince description**

Budget Amount variance uses the calculation from Sales Amount and Budget Amount and calculates the difference between the two.

**Usage scenario(s)**

Budget Amount Variance can be used in scenarios where you would want to compare how sales are performing against a budget.
**Calculation**

Budget Amount Varaince  is calculated as follows: The sum of Budget Amount from the Item Budget Entries divided by the Sales Amount from the Sales table.

**Data source(s)**

To calculate Revenue, data from the following tables is used: 
- Item Budget Entries
- Sales

### Budget Amount Variance %

**Budget Amount Variance % description**

Budget Amount Variance % is used to highlight the budget vs sales varaince as a percentage value.


**Usage scenario(s)**

You can use Budget Amount Variance % to highlight the variance in sales vs budget as a percentage value.

**Calculation**

Budget Amount Varaince % is calculated as follows: The sum of Budget Amount from the Item Budget Entries divided by the Sales Amount from the Sales table.

**Data source(s)**

To calculate Revenue, data from the following tables is used: 
- Item Budget Entries
- Sales

### Budget Quantity

**Budget Quantity description**

Budget Quantity metric to indicidate the quanity on a specific budget based on your filtering.

**Usage scenario(s)**

You can use Budget Quantity to highlight the specifc value of a specific budget and a period of time.

**Calculation**

Budget Quantity is calculated as follows: The sum of Sales Quantity from the Item Budget Entries.

**Data source(s)**

To calculate Budget Quantity, data from the following tables is used: 
- Item Budget Entries

### Budget Quantity Variance

**Budget Quantity Variance description**

Budget Quantity Varaince is a measure to highlight the quantity differnce between the Sales Quantity against the Budget Quantity.

**Usage scenario(s)**

You can use Budget Quantity Varaince to show the difference between the Sales Quantity and Budgetted Quantity. This can be good to highlight the specifc areas where more effort for Sales might be required.

**Calculation**

Budget Amount is calculated as follows: The sum of Sales Amount from the Item Budget Entries.

**Data source(s)**

To calculate Revenue, data from the following tables is used: 
- Item Budget Entries
- Sales

### Budget Quantity Variance %

**Budget Quantity description**

Budget Quantity Variance % is used to show the variance between Sales Quantity and Budget Quantity as a percentage value.

**Usage scenario(s)**

You can use this measure to as a performance indictor to see things are tracking for Sales.

**Calculation**

Budget Quantity Variance % is calculated as follows: The divide of Sales Quantity from Sales and the Budget Quantity from teh Item Budget Entries.

**Data source(s)**

To calculate Budget Quantity Variance %, data from the following tables is used: 
- Item Budget Entries
- Sales



## Data foundation for the Power BI reports on finance

The Power BI reports on finance is based on the following tables in Business Central:

- Table 1
- Table 2


<!-- ## See also -->

