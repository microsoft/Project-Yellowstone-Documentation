# Moving Annual Total (MAT) (Power BI Report)

The _Moving Annual Total (MAT)_ report calculates a total of purchase over the last 12 months. This is a rolling calculation where the date is continual moving. This report will showcase the Purchase Amount MAT and compare this against the MAT for the previous period. 

This report is ideal for business leaders and purchasing managers who need to monitor their purchase performance in the last 12 months.

//TODO: insert report screenshot

## What the report shows

The *Moving Annual Total* reports shows a bar graph for moving annual totals over time and a drill-through table for detailed monthly analysis of moving annual total and how it compares to the previous year moving annual totals.

## Use Cases

For the Team:

**Target Audience**
- Leadership Role 1
- Leadership Role 2

**Example Scenario:** As a specific role, I want to ...

---

## Key Performance Indicators (KPIs)

The _Moving Annual Total_ report includes the following KPIs:

- **MAT**
- **PYMAT**
- **MAT Growth**
- **MAT Growth %**

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

---
## Key Performance Indicators (KPIs)

The _Moving Annual Total_ report includes the following KPIs:

- [**Moving Annual Total (MAT)**](#moving-annual-total-mat)
- [**Previous Year Moving Annual Total (PYMAT)**](#previous-year-moving-annual-total-pymat)
- [**Moving Annual Total Growth Amount**](#moving-annual-total-growth-amount)
- [**Moving Annual Total Growth %**](#moving-annual-total-growth-)
- [**Purchase Amount**](#purchase-amount)

---
### Moving Annual Total (MAT)
The *Moving Annual Total (MAT)* shows the rolling sum of purchase amounts in the last 12 months.

**Formula**  

*Moving Annual Total (MAT)* is the sum of purchase amounts from all purchase value entries in the last 12 months.

**Data Sources**

Data from the following tables are used to calculate the *Moving Annual Total (MAT)*:
- Value Entry

---
### Previous Year Moving Annual Total (PYMAT)
The *Previous Year Moving Annual Total (PYMAT)* shows the rolling sum of purchase amounts in the last 12 months of the previous year. 

For example, if the current MAT represents data between December 2022 to November 2023, the PYMAT shows data between December 2021 to November 2022.

**Formula**  

*Previous Year Moving Annual Total (PYMAT)* is the sum of purchase amounts from all purchase value entries in the last 12 months of the previous year.

**Data Sources**

Data from the following tables are used to calculate the *Previous Year Moving Annual Total (PYMAT)*:
- Value Entry

---
### Moving Annual Total Growth Amount
The *Moving Annual Total Growth Amount* shows the change in the purchase amount between the moving annual total and the previous year moving annual total.

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
### Purchase Amount

The *Purchase Amount* shows the total purchase amount earned within a specific time period.

**Formula**  

*Purchase Amount* is the total amount of all value entries related to purchase is added up for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Purchase Amount*:
- Value Entry

## Data used in the Moving Annual Total report

Data from the following tables are used on the *Moving Annual Total* report
- Value Entry
- Purchase Line

## See also
