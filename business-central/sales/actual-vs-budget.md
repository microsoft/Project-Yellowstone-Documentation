# Actual vs. Budget (Power BI Report)

The _Actual vs. Budget_ report provides a clear overview of your organization's sales performance by comparing actual sales amount and quantity sold with the budget figures. This report helps the organization to track progress towards meeting sales targets and analyze sales data by item categories and items for making key business decisions.


This report is meant for finance and sales teams to track performance of actual sales against budgets.

![Sales Actual vs. Budget screenshot](/business-central/media/sales/sales-actual-vs-budget.png "Sales Actual vs. Budget - Screenshot")

## What the report shows

The _Actual vs. Budget_ report shows the actual sales quantities and amounts and how they are tracking against the sales budget. Specifically, the report provides insights into how specific item categories and items are tracking against their budget and highlights the variance amount and percentage.

## Use Cases

For the Leadership Team:

The CEO of a retail company can use the _Actual vs. Budget_ report to ensure the sales targets are being met and understand how the sales performance of the entire organization are tracking against their budget. This report helps the CEO to make informed decisions for managing the budget.

**Target Audience**
- CEO
- Head of Sales

---

For the Management Team:

The Sales Manager of a retail store wants to analyze sales data to make decisions about inventory management. By analyzing the Variance and Budget Amount Variance indicators, the manager can see how the specific item categories and items are tracking against their allocated budget. This report helps the manager to understand which items are selling well and which items need to be restocked or discontinued.

**Target Audience**

- Sales Manager
- Business Development Manager

---

For the Sales Team:

A salesperson at a retail store wants to ensure that he is meeting his sales targets. Using the _Actual vs. Budget_ report, he can see the sales performance of the specific item categories and items he is responsible for selling. This report helps him to understand the budget amount and variance figures and where he may need to focus his efforts to improve his sales performance.

**Target Audience**

- Salesperson
- Sales Representative

## Key Performance Indicators (KPIs)

The _Actual vs. Budget_ report includes the following KPIs:

- [**Sales Quantity**](#sales-quantity)  
- [**Sales Amount**](#sales-amount)  
- [**Budget Quantity**](#budget-quantity)  
- [**Budget Amount**](#budget-amount)  
- [**Budget Amount Variance**](#budget-amount-variance)  
- [**Budget Amount Variance %**](#budget-amount-variance-)  
- [**Variance**](#variance)  
- [**Variance %**](#variance-)  

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

---
### Sales Quantity

The *Sales Quantity* is the total number of items sold within a specific time period.

**Formula**  

*Sales Quantity* is the quantity of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry

---
### Sales Amount

The *Sales Amount* is the actual amount of items sold within a specific time period. This amount represents the net sales amount in local currency, excluding VAT.

**Formula**  

*Sales Amount* is the actual amount of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry

---
### Budget Quantity

The *Budget Quantity* is the total quantity of items allocated for a specific time period.

**Formula**  

*Budget Quantity* is the total quantity based on the item budget entries for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Budget Quantity*:
- Item Budget Entry

---
### Budget Amount

The *Budget Amount* is the total amount of money allocated for items during a specific time period.

**Formula**  

*Budget Amount* is the total amount based on the item budget entries for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Budget Amount*:
- Item Budget Entry

---
### Budget Amount Variance

The **Budget Amount Variance** shows the difference between the actual sales amount and the budget amount.This metric helps to track the performance of the actual sales against the budgeted amount.

**Formula**  

*Budget Amount Variance* = Sales Amount - Budget Amount

**Data Sources**

Data from the following tables are used to calculate the *Budget Amount Variance*:
- Value Entry
- Item Budget Entry

---
### Budget Amount Variance %

The *Budget Amount Variance %* shows the variance amount as a percentage of the budget amount.

**Formula**  

*Budget Amount Variance %* = (Budget Amount Variance / Budget Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Budget Amount Variance %*:
- Value Entry
- Item Budget Entry

---
### Variance

The **Variance** shows the difference between the actual sales quantity and the budget quantity. This metric helps to track the performance of the actual quantity sold against the budgeted quantity.

**Formula**  

*Variance* = Sales Quantity - Budget Quantity

**Data Sources**

Data from the following tables are used to calculate the *Variance*:
- Value Entry
- Item Budget Entry

---
### Variance %

The *Variance %* shows the variance quantity as a percentage of the budget quantity.

**Formula**  

*Variance %* = (Variance / Budget Quantity) x 100

**Data Sources**

Data from the following tables are used to calculate the *Variance %*:
- Value Entry
- Item Budget Entry


## Data used in the Actual vs. Budget report

Data from the following tables are used on the *Actual vs. Budget* report
- Item
- Item Category
- Value Entry
- Sales Line
- Item Budget Entry


## See also
