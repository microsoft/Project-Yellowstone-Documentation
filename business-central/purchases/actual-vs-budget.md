# Actual vs. Budget (Power BI Report)

The _Actual vs. Budget_ report provides a clear overview of your organization's purchase performance by comparing actual purchase amount and quantity with the budget figures. This report allows users to analyze and monitor purchase data by item categories and items, providing a detailed view of purchase budget and variance.

This report is meant for purchase and finance teams to track actual spendings against budgets.

// TODO: insert report screenshot

## What the report shows

The _Actual vs. Budget_ report shows the actual purchase quantities and amounts and how they are tracking against the purchase budget. Specifically, the report provides insights into how specific item categories and items are tracking against their budget and highlights the variance amount and percentage.

## Use Cases

For the Team:

**Target Audience**
- Leadership Role 1
- Leadership Role 2

**Example Scenario:** As a specific role, I want to ...

---

## Key Performance Indicators (KPIs)

The _Actual vs. Budget_ report includes the following KPIs:

- [**Purchase Quantity**](#purchase-quantity)  
- [**Purchase Amount**](#purchase-amount)  
- [**Budget Quantity**](#budget-quantity)  
- [**Budget Amount**](#budget-amount)  
- [**Budget Amount Variance**](#budget-amount-variance)  
- [**Budget Amount Variance %**](#budget-amount-variance-)  
- [**Variance**](#variance)  
- [**Variance %**](#variance-)  

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

---
### Purchase Quantity

The *Purchase Quantity* is the total number of items purchased within a specific time period.

**Formula**  

*Purchase Quantity* is the quantity of all value entries related to purchase for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Purchase Quantity*:
- Value Entry

---
### Purchase Amount

The *Purchase Amount* is the actual amount of items purchased within a specific time period. This amount represents the net purchase amount in local currency, excluding VAT.

**Formula**  

*Purchase Amount* is the actual amount of all value entries related to purchase for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Purchase Amount*:
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

The *Budget Amount Variance* shows the difference between the actual purchase amount and the budget amount.

**Formula**  

*Budget Amount Variance* = Purchase Amount - Budget Amount

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

The _Variance_ shows the difference between the actual purchase quantity and the budget quantity.

**Formula**  

*Variance* = Purchase Quantity - Budget Quantity

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
- Purchase Line
- Item Budget Entry


## See also
