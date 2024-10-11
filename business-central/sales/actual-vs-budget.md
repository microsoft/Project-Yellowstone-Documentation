# Actual vs. Budget (Power BI Report)

The _Actual vs. Budget_ report gives a clear picture of your organization's sales activities and how these are tracking against the sales budget. It showcases the sales amounts and quantities and the counterparts of these as budget amount and quantity. This report can provide a clear picture for organizations about how specific Item Categories and Items are tracking against their budget. This can allows key decisions to be made in improving sales ensuring budget figures are met. 

This report is meant for finance and sales teams to track performance of sales against budgets.

//ACTUAL VS BUDGET IMAGE

## What the report shows

The _Actual vs. Budget_ report shows the actual sales quantities and amounts and how they are tracking against the sales budget. Specifically, the report provides insights into how specific item categories and items are tracking against their budget and highlights the variance amount and percentage.


## Use Cases for Actual vs. Budget

For the Leadership Team, the *Actual vs. Budget* report helps to track the overall performance against the organizational goals and to make informed decisions.

**Target Audience**
- CEO
- Head of Sales & Marketing
- Head of Finance

**Example Scenario:** A Head of Sales & Marketing wants to monitor the sales activities and track how it is tracking against the budget. The *Actual vs. Budget* report provides them with a clear picture of sales figures and helps them identify areas of improvement for budget allocation.

---

For the Management Team, the *Actual vs. Budget* report serves as a valuable tool to monitor sales activities and track actual sales figures against budgets. This report helps them to identify potential areas where sales are exceeeding or falling short of expections by analyzing the variance figures.

**Target Audience**

- Sales Manager
- Regional Sales Manager
- Business Development Manager

**Example Scenario**: A Business Development Manager needs to identify new business opportunities and expand the customer base. The *Actual vs. Budget* report provides them with accurate data to make decisions about sales strategies and which item categories to focus on.

---

For the Sales team,the *Actual vs. Budget* report ...

**Target Audience**

- Salesperson
- Sales Representative

**Example Scenario:** A Salesperson needs to promote and sell products to the customers. The *Actual vs. Budget* report helps them track their sales figures of each item category against sales budgets and identify which products to promote to meet their sales KPIs.


## Key Performance Indicators (KPIs)

The _Actual vs. Budget_ report includes the following KPIs:

- [**Sales Quantity**](#sales-quantity)  
- [**Sales Amount**](#sales-amount)  
- [**Budget Quantity**](#budget-quantity)  
- [**Budget Amount**](#budget-amount)  
- [**Budget Amount Variance**](#budget-amount-variance)  
- [**Budget Amount Variance %**](#budget-amount-variance-)  
- [**Variance**](#Variance)  
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
