# Sales KPIs

This page provides a list of all KPIs included in the Power BI Sales Report. Explore the list of KPIs below to learn more about how they can help you achieve your business goals.

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

The *Budget Amount Variance* shows the difference between the actual sales amount and the budget amount.

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

The *Variance* shows the difference between the actual sales quantity and the budget quantity. 

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

---
### Sales Amount

The *Sales Amount* shows the total sales revenue earned in the current year. This KPI enables you to track your total sales revenue for the year thus far.

**Formula**  

*Sales Amount* is the total amount of all value entries related to sales is added up for the selected year.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry

---
### Sales Amount MTD

The *Sales Amount MTD* is the total sales amount earned in the current month, up until yesterday.

**Formula**  

*Sales Amount MTD* is the total amount of all value entries related to sales is added up for the selected month, excluding today's date. 

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount MTD*:
- Value Entry

---
### Gross Profit MTD

The *Gross Profit MTD* is the gross profit earned in the current month, up until yesterday.

**Formula**  

*Gross Profit MTD* is the total gross profit amount of all value entries related to sales is added up for the selected month, excluding today's date.

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit MTD*:
- Value Entry

---
### Sales Quantity

The *Sales Quantity* is the total number of items sold within a specific time period.

**Formula**  

*Sales Quantity* is the quantity of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry
- Sales Line

---
### Sales Amount

The *Sales Amount* is the actual amount of items sold within a specific time period. This amount represents the net sales amount in local currency, excluding VAT.

**Formula**  

*Sales Amount* is the actual amount of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry
- Sales Line

---
### Cost Amount

The *Cost Amount* represents the total cost of goods sold incured by a location within a specific time period.

**Formula**  

*Cost Amount* is the the total cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount*:
- Value Entry
- Sales Line

---
### Gross Profit

The *Gross Profit* shows the difference between the sales revenue and the cost of goods sold for a location within a specifict time period.

**Formula**  

*Gross Profit* = Sales Amount - (Cost Amount + Cost Amount Non-Inv) 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry
- Sales Line

---
### Gross Profit Margin

The *Gross Profit Margin* shows the gross profit as a percentage over the sales amount.

**Formula**  

*Gross Profit Margin* = (Gross Profit / Sales Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit Margin*:
- Value Entry
- Sales Line

---
### Moving Annual Total (MAT)
The *Moving Annual Total (MAT)* shows the rolling sum of sales amounts in the last 12 months.

**Formula**  

*Moving Annual Total (MAT)* is the sum of sales amounts from all sales value entries in the last 12 months.

**Data Sources**

Data from the following tables are used to calculate the *Moving Annual Total (MAT)*:
- Value Entry

---
### Previous Year Moving Annual Total (PYMAT)
The *Previous Year Moving Annual Total (PYMAT)* shows the rolling sum of sales amounts in the last 12 months of the previous year. 

For example, if the current MAT represents data between December 2022 to November 2023, the PYMAT shows data between December 2021 to November 2022.

**Formula**  

*Previous Year Moving Annual Total (PYMAT)* is the sum of sales amounts from all sales value entries in the last 12 months of the previous year.

**Data Sources**

Data from the following tables are used to calculate the *Previous Year Moving Annual Total (PYMAT)*:
- Value Entry

---
### Moving Annual Total Growth Amount
The *Moving Annual Total Growth Amount* shows the change in the sales amount between the moving annual total and the previous year moving annual total.

**Formula**  

*Moving Annual Total Growth Amount* = Moving Annual Total - Previous Year Moving Annual Total

**Data Sources**

Data from the following tables are used to calculate the *Moving Annual Total Growth Amount*:
- Value Entry

---
### Moving Annual Total Growth %
The *Moving Annual Total Growth %* shows the moving annual total growth amount as a percentage of the previous year moving annual total.

**Formula**  

*Moving Annual Total Growth %* = (Moving Annual Total Growth Amount / Previous Year Moving Annual Total) x 100

**Data Sources**

Data from the following tables are used to calculate the *Moving Annual Total Growth %*:
- Value Entry

---
### Sales Amount

The *Sales Amount* shows the total sales amount earned within a specific time period.

**Formula**  

*Sales Amount* is the total amount of all value entries related to sales is added up for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry

### Sales Amount

The *Sales Amount* represents the total revenue generated by a location from all sales activities within a specific time period.

**Formula**  

*Sales Amount* is the total amount of all value entries related to sales from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry
- Sales Line

---
### Sales Amount Average 30D

The *Sales Amount Average 30D* represents the total revenue generated by a location from all sales activities within a specific time period.

**Formula**  

*Sales Amount* is the total amount of all value entries related to sales from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry
- Sales Line

---
### Sales Amount

The *Sales Amount* shows the total sales amount earned in the current period.

**Formula**  

*Sales Amount* is the total amount of all value entries related to sales is added up for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry

---
### Previous Period

The *Previous Period* shows the total sales amount earned in the previous period. For example, if the current *Sales Amount* is January 2023, the *Previous Period* shows the sales amount in January 2022.

**Formula**  

*Previous Period* is the total amount of all value entries related to sales is added up for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Previous Period*:
- Value Entry

---
### Previous Period

The *Previous Period* shows the total sales amount earned in the previous period. For example, if the current *Sales Amount* captures the sales amount in January 2023, the *Previous Period* shows the sales amount in January 2022.

**Formula**  

*Previous Period* is the total amount of all value entries related to sales is added up for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Previous Period*:
- Value Entry

---
### Period-over-Period Growth Amount

The *Period-over-Period Growth Amount* is the change in the total amount between the current period and previous period.

**Formula**  

*Period-over-Period Growth Amount* = Sales Amount - Previous Period

**Data Sources**

Data from the following tables are used to calculate the *Period-over-Period Growth Amount*:
- Value Entry

---
### Period-over-Period Growth %

The *Period-over-Period Growth %* shows the period-over-period growth amount as a percentage of the current sales amount.

**Formula**  

*Period-over-Period Growth %* = (Period-over-period Growth Amount / Sales Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Period-over-Period Growth %*:
- Value Entry

---
### Sales Quantity

The *Sales Quantity* is the total number of items sold within a specific time period.

**Formula**  

*Sales Quantity* is the quantity of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry
- Sales Line

---
### Sales Amount

The *Sales Amount* is the actual amount of items sold within a specific time period. This amount represents the net sales amount in local currency, excluding VAT.

**Formula**  

*Sales Amount* is the actual amount of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry
- Sales Line

---
### Cost Amount

The *Cost Amount* represents the total cost of goods sold incured by a location within a specific time period.

**Formula**  

*Cost Amount* is the the total cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount*:
- Value Entry
- Sales Line
---
### Cost Amount Non-Inv

The *Cost Amount Non-Inv* represents the total cost of non-inventory items by a location within a specific time period. These costs include expenses such as freight costs, shipping costs, marketing expenses, or any other indirect costs associated with sales.

**Formula**  

*Cost Amount Non-Inv* is the the total non-inventory cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount Non-Inv*:
- Value Entry
- Sales Line

---
### Gross Profit

The *Gross Profit* shows the difference between the sales revenue and the cost of goods sold for a location within a specifict time period.

**Formula**  

*Gross Profit* = Sales Amount - (Cost Amount + Cost Amount Non-Inv) 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry
- Sales Line

---
### Gross Profit Margin

The *Gross Profit Margin* shows the gross profit as a percentage over the sales amount.

**Formula**  

*Gross Profit Margin* = (Gross Profit / Sales Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit Margin*:
- Value Entry
- Sales Line

---
### Sales Quantity

The *Sales Quantity* is the total number of items sold within a specific time period.

**Formula**  

*Sales Quantity* is the quantity of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry
- Sales Line

---
### Sales Amount

The *Sales Amount* is the actual amount of items sold within a specific time period. This amount represents the net sales amount in local currency, excluding VAT.

**Formula**  

*Sales Amount* is the actual amount of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry
- Sales Line

---
### Cost Amount

The *Cost Amount* represents the total cost of goods sold incured by a location within a specific time period.

**Formula**  

*Cost Amount* is the the total cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount*:
- Value Entry
- Sales Line

---
### Cost Amount Non-Inv

The *Cost Amount Non-Inv* represents the total cost of non-inventory items by a location within a specific time period. These costs include expenses such as freight costs, shipping costs, marketing expenses, or any other indirect costs associated with sales.

**Formula**  

*Cost Amount Non-Inv* is the the total non-inventory cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount Non-Inv*:
- Value Entry
- Sales Line

---
### Gross Profit

The *Gross Profit* shows the difference between the sales revenue and the cost of goods sold for a location within a specifict time period.

**Formula**  

*Gross Profit* = Sales Amount - (Cost Amount + Cost Amount Non-Inv) 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry
- Sales Line

---
### Gross Profit Margin

The *Gross Profit Margin* shows the gross profit as a percentage over the sales amount.

**Formula**  

*Gross Profit Margin* = (Gross Profit / Sales Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit Margin*:
- Value Entry
- Sales Line

---
### Sales Amount

The *Sales Amount* represents the total revenue generated by a location from all sales activities within a specific time period.

**Formula**  

*Sales Amount* is the total amount of all value entries related to sales from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry

---
### Sales Quantity

The *Sales Quantity* represents the total quantity sold by a location from all sales activities within a specific time period.

**Formula**  

*Sales Quantity* is the total quantity of all value entries related to sales from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry

---
### Cost Amount

The *Cost Amount* represents the total cost of goods sold incured by a location within a specific time period.

**Formula**  

*Cost Amount* is the the total cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount*:
- Value Entry

---
### Cost Amount Non-Inv

The *Cost Amount Non-Inv* represents the total cost of non-inventory items by a location within a specific time period. These costs include expenses such as freight costs, shipping costs, marketing expenses, or any other indirect costs associated with sales.

**Formula**  

*Cost Amount Non-Inv* is the the total non-inventory cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount Non-Inv*:
- Value Entry

---
### Gross Profit

The *Gross Profit* shows the difference between the sales revenue and the cost of goods sold for a location within a specifict time period.

**Formula**  

*Gross Profit* = Sales Amount - (Cost Amount + Cost Amount Non-Inv) 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry

---
### Gross Profit Margin

The *Gross Profit Margin* shows the gross profit as a percentage over the sales amount.

**Formula**  

*Gross Profit Margin* = (Gross Profit / Sales Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit Margin*:
- Value Entry

---
### Sales Amount

The *Sales Amount* represents the total revenue generated by a salesperson from all sales activities within a specific time period.

**Formula**  

*Sales Amount* is the total amount of all value entries related to sales from the salesperson for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry

---
### Sales Quantity

The *Sales Quantity* represents the total quantity sold by a salesperson from all sales activities within a specific time period.

**Formula**  

*Sales Quantity* is the total quantity of all value entries related to sales from the salesperson for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry

---
### Gross Profit

The *Gross Profit* shows the difference between the sales revenue and the cost of goods sold for a salesperson within a specific time period.

**Formula**  

*Gross Profit* = Sales Amount - Cost Amount 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry

---
### Gross Profit Margin

The *Gross Profit Margin* shows the gross profit as a percentage over the sales amount.

**Formula**  

*Gross Profit Margin* = (Gross Profit / Sales Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit Margin*:
- Value Entry
