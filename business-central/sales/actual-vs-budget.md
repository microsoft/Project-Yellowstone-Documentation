# Actual vs. Budget (Power BI Report)

The _Actual vs. Budget_ report provides a clear overview of your organization's sales performance by comparing actual sales amount and quantity sold with the budget figures. This report helps the organization to track progress towards meeting sales targets and analyze sales data by item categories and items for making key business decisions.


This report is meant for finance and sales teams to track performance of actual sales against budgets.

![Sales Actual vs. Budget screenshot](/business-central/media/sales/sales-actual-vs-budget.png "Sales Actual vs. Budget - Screenshot")

## What the report shows

The _Actual vs. Budget_ report shows the actual sales quantities and amounts and how they are tracking against the sales budget. Specifically, the report provides insights into how specific item categories and items are tracking against their budget and highlights the variance amount and percentage.

## Use Cases

For the Leadership Team:

**Target Audience**
- CEO
- Head of Sales

**Example Scenario:** As a CEO of a retail company, you can easily track and compare your sales performance against your budget to ensure that your sales targets are being met. This report provides a comprehensive overview of the entire organization's sales performance, allowing you to make informed decisions when managing your budget.

---

For the Management Team:

**Target Audience**

- Sales Manager
- Business Development Manager

**Example Scenario:** As a Sales Manager of a retail store, you can use this report to analyze your sales data and make decisions about inventory management. By analyzing the Variance and Budget Amount Variance indicators in the report, you can see how specific item categories and items are tracking against their allocated budget. This report will help you to understand which items are selling well and which ones need to be restocked or discontinued. With this information, you can optimize your inventory and ensure that your store is always stocked with the products that your customers want to buy.

---

For the Sales Team:

**Target Audience**

- Salesperson
- Sales Representative

**Example Scenario:** As a Salesperson of a retail company, you can monitor the variance metrics to ensure that you are meeting your sales targets. This report allows you to see the sales performance of the specific item categories and items that you are responsible for selling. By analyzing the budget amount and variance figures in the report, you can understand where you may need to focus your efforts to improve your sales performance. With this information, you can identify areas of opportunity to increase sales and optimize your approach to selling specific items, helping you to meet and exceed your sales targets.

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
