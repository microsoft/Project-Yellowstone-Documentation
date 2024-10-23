# Period-Over-Period (Power BI Report)

The _Period-Over-Period Growth_ report provides valuable insights into your organization's purchasing performance over time. This report compares purchasing amounts for different time periods to the same period in the previous year, allowing you to  identify growth trends and areas for improvement.

For instance, if the analysis scope is fiscal months, the report compares the purchasing amount in October 2023 to the purchasing amount in October 2022, and if the analysis scope is fiscal years, the report compares the purchasing amount in FY 2023 to the purchasing amount in FY 2022.

This report is meant for business leaders and purchasing managers. 

## What the report shows

The _Period-Over-Period Growth_ reports shows a bar graph for comparison of sales amounts between the current year and the previous year and a drill-through table for detailed monthly analysis.

## Use Cases

For the Team:

**Target Audience**
- Leadership Role 1
- Leadership Role 2

**Example Scenario:** As a specific role, I want to ...

---

## Key Performance Indicators (KPIs)

The _Period-Over-Period_ report includes the following KPIs:

- [**Purchase Amount**](#purchase-amount)  
- [**Previous Period**](#previous-period)  
- [**Period-over-Period Growth Amount**](#period-over-period-growth-amount)  
- [**Period-over-Period Growth %**](#period-over-period-growth-)  

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

---
### Purchase Amount

The *Purchase Amount* is the actual amount of items purchased within a specific time period. This amount represents the net purchase amount in local currency, excluding VAT.

**Formula**  

*Purchase Amount* is the actual amount of all value entries related to purchase for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Purchase Amount*:
- Value Entry

---
### Previous Period

The *Previous Period* shows the total purchase amount earned in the previous period. For example, if the current *Purchase Amount* captures the purchase amount in January 2023, the *Previous Period* shows the purchase amount in January 2022.

**Formula**  

*Previous Period* is the total amount of all value entries related to purchase is added up for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Previous Period*:
- Value Entry

---
### Period-over-Period Growth Amount

The *Period-over-Period Growth Amount* is the change in the total amount between the current period and previous period.

**Formula**  

*Period-over-Period Growth Amount* = Purchase Amount - Previous Period

**Data Sources**

Data from the following tables are used to calculate the *Period-over-Period Growth Amount*:
- Value Entry

---
### Period-over-Period Growth %

The *Period-over-Period Growth %* shows the period-over-period growth amount as a percentage of the current purchase amount.

**Formula**  

*Period-over-Period Growth %* = (Period-over-period Growth Amount / Purchase Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Period-over-Period Growth %*:
- Value Entry


## Data used in the Period-Over-Period report

Data from the following tables are used on the *Period-Over-Period* report
- Table 1
- Table 2

## See also
