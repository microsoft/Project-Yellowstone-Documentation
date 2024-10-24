# Purchases By Location (Power BI Report)

The _Purchases by Location_ report provides an overview of purchasing activities by location. This report allows you to analyze which item categories and items are most frequently purchased in each location, as well as how much money is being spent on these purchases.

This report is especially useful for purchasing managers and purchasers who need to closely monitor their organization's purchasing activities. By using this report, you can gain insights into purchasing trends and make informed decisions about future purchasing activities across your locations.

## What the report shows

The _Purchases By Location_ report displays a treemap of the most frequently purchased items, a table of purchases by location, and a bar chart that breaks down purchases by items. These visuals provide insights into the distribution of purchases across different item categories and helps you identify any areas that require attention.


## Use Cases

For the Team:

**Target Audience**
- Leadership Role 1
- Leadership Role 2

**Example Scenario:** As a specific role, I want to ...

---

## Key Performance Indicators (KPIs)

The _Purchases By Location_ report includes the following KPIs:

- **Purchase Amount**
- **Purchase Quantity**
- **% GT Purchase Amount**
- **% GT Purchase Quantity**

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

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

## Data used in the Purchases By Location report

Data from the following tables are used on the *Purchases By Location* report
- Location
- Item
- Value Entry
- Purchase Line


## See also
