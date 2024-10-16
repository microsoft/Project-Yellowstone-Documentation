# Moving Annual Total (Power BI Report)

The _Moving Annual Total (MAT)_ report calculates a total of sales over the last 12 months. This is a rolling calculation where the date is continual moving. This report will showcase the Sales Amount MAT and compare this against the MAT for the previous period. 

This report is meant for business leaders and managers to identify how the MAT is performing across the period.

![Sales Moving Annual Total screenshot](/business-central/media/sales/sales-moving-annual-total.png "Sales Moving Annual Total - Screenshot")

## What the report shows

The *Moving Annual Total* reports shows a bar graph for moving annual totals over time and a drill-through table for detailed monthly analysis of moving annual total and how it compares to the previous year moving annual totals.

## Use Cases

A CEO can use this report to keep track of the sales performance in the last 12 months and come up with a strategic plan for the upcoming year to increase the company's sales and profits. For example, the CEO might realize that the company's sales have been declining after the company's competitor introduced a new product in the market. The CEO can make informed decisions to allocate more resources to the region to improve the company's sales and better compete with the competitor.


**Target Audience**

- CEO
- COO

---

For the Management Team:

The Sales Manager of a retail company can use this report to see how sales have been performing over the last 12 months. The manager might notice that the sales of a particular category of items have been declining over the last few months. The manager can drill down to the monthly analysis to see when the sales started to decline. After analyzing the data, the manager can take actions to introduce items that align with the new trend to increase sales and meet customer demand.

**Target Audience**

- Sales Manager
- Finance Manager


## Key Performance Indicators (KPIs)

The _Moving Annual Total_ report includes the following KPIs:

- [**Moving Annual Total (MAT)**](#moving-annual-total-mat)
- [**Previous Year Moving Annual Total (PYMAT)**](#previous-year-moving-annual-total-pymat)
- [**Moving Annual Total Growth Amount**](#moving-annual-total-growth-amount)
- [**Moving Annual Total Growth %**](#moving-annual-total-growth-)
- [**Sales Amount**](#sales-amount)

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

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

## Data used in the Moving Annual Total report

Data from the following tables are used on the *Moving Annual Total* report
- Value Entry
- Sales Line

## See also
