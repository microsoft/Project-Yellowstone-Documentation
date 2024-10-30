# Purchases By Item (Power BI Report)

The _Purchases by Item_ report gives a clear picture of your organization's item purchases. It showcases key metrics against each item or item category such as purchase amount and quantities along with the cost amounts.

## How to use the report

This report is targetted towards the purchasing department who want to closely monitor the organization's purchasing activities. 

As a purchasing manager, you want to have a clear understanding of the organization's purchasing activities and how they align with the overall business goals. You can use the *Purchases by Item* report to track the purchase amounts and quantities against each item or item category. You can also use this report to identify any discrepancies or anomalies in the purchasing data and take necessary actions to optimize the purchasing process and reduce costs.

As a purchaser, you are responsible for making purchasing decisions for specific items or categories. You want to ensure that you are making informed decisions and getting the best value for the organization. You can use this report to track the purchase amounts and quantities of the items or categories you are responsible for.

---

## Key Performance Indicators (KPIs)

The _Purchases By Item_ report includes the following KPIs:

- [**Purchase Amount**](#purchase-amount)
- [**Purchase Quantity**](#purchase-quantity)
- [**% GT Purchase Amount**](#-gt-purchase-amount)
- [**% GT Purchase Quantity**](#-gt-purchase-quantity)

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
### Purchase Quantity

The *Purchase Quantity* is the total number of items purchased within a specific time period.

**Formula**  

*Purchase Quantity* is the quantity of all value entries related to purchase for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Purchase Quantity*:
- Value Entry
- Purchase Line

---
### % GT Purchase Amount

The *% GT Purchase Amount*, abbreviated for *Percentage of Grand Total Purchase Amount*, is the percentage of the total purchase amount during a specific time period.

**Formula**  

*% GT Purchase Amount* = (*Purchase Amount* / Grand Total Purchase Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *% GT Purchase Amount*:
- Value Entry
- Purchase Line

---
### % GT Purchase Quantity

The *% GT Purchase Quantity*, abbreviated for *Percentage of Grand Total Purchase Quantity*, is the percentage of the total purchased quantity during a specific time period.

**Formula**  

*% GT Purchase Quantity* = (*Purchase Quantity* / Grand Total Purchase Quantity) x 100

**Data Sources**

Data from the following tables are used to calculate the *% GT Purchase Quantity*:
- Value Entry
- Purchase Line

## Data used in the Purchases By Item report

Data from the following tables are used on the *Purchases By Item* report
- Value Entry
- Purchase Line


## See also
