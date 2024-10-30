# Purchases By Vendor (Power BI Report)

The Purchases by Vendor report provides an overview of purchasing activities by vendor. This report allows you to analyze which vendors are supplying the most frequently purchased item categories and items, as well as how much money is being spent on these purchases.

## How to use the report

This report is especially useful for purchasing managers and purchasers .

As a purchasing manager, you can use the *Purchases by Vendor* report to analyze vendor performance. You can then identify the vendors who supply the most frequently purchased item categories and items. This information can help you optimize your purchasing strategies, negotiate better prices, and improve your overall vendor management.

As a purchaser, you can use this report to monitor purchasing activities and identify the suppliers of specific products. For example, if you need to find a list of suppliers for the company components to assemble dining chairs, you can view the purchase quantities and amounts spent on each vendor. The report analysis can help you select the best vendor to buy from.

---

## Key Performance Indicators (KPIs)

The _Purchases By Vendor_ report includes the following KPIs:

- **Purchase Amount**
- **Purchase Quantity**
- **% GT Purchase Amount**
- **% GT Purchase Amount PY (Fiscal)**

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


## Data used in the Purchases By Vendor report

Data from the following tables are used on the *Purchases By Vendor* report
- Vendor
- Item
- Value Entry
- Purchase Line


## See also
