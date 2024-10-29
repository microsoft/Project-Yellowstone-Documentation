# Actual vs. Budget (Power BI Report)

The *Actual vs. Budget* report provides a clear overview of your organization's purchase performance by comparing actual purchase amount and quantity with the budget figures. This report allows you to analyze and monitor purchase data by item categories and items, providing a detailed view of purchase budget and variance.

**// TODO: insert report screenshot**

## How to use the report

The *Actual vs. Budget* report is meant for purchase and finance teams to track actual spendings against budgets.

As a CEO, you can easily track and analyze the purchasing performance of your organization against your budget to ensure that you are meeting your financial goals. This report provides a comprehensive overview of the entire organization's purchasing performance, allowing you to make informed decisions when managing your budget. With this report, you can identify areas where your organization is overspending or underspending, and adjust your purchasing budget accordingly.  
   
As a purchasing manager, you can use this report to analyze your purchasing data and make decisions about inventory management. By analyzing the Variance and Budget Amount Variance indicators in the report, you can see how specific item categories and items are tracking against their allocated budget. This report will help you to understand which items are being purchased frequently and which ones are not, allowing you to optimize your inventory and ensure that your organization is always stocked with the products that you need.  
   
As a purchaser, you can monitor the variance metrics to ensure that you are meeting your purchasing targets. This report allows you to see the purchasing performance of the specific item categories and items that you are responsible for purchasing. With this information, you can identify areas of opportunity to reduce costs and optimize your approach to purchasing specific items.

## Key Performance Indicators (KPIs)

The *Actual vs. Budget* report includes the following KPIs:

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
