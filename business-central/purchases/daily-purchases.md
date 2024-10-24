# Daily Purchase (Power BI Report)

The _Daily Purchase_ report provides a comprehensive overview of your organization's purchase activities on specific days. By highlighting days with a higher volume of purchases, you can identify trends and patterns in your purchasing behavior. This report can also be used to analyze purchase data across different years, quarters, or months, providing valuable insights into purchasing trends over time.

This report is designed for purchasing managers looking to optimize purchasing schedules and purchasing teams looking to track daily purchase activities.

// TODO: insert report screenshot

## What the report shows

The _Daily Purchases_ report displays the daily purchase amount for each date, allowing users to identify days with high and low demand. The report presents this data in both a matrix view and a standard table view. Users can drill down into the Purchase Drillthrough page to access more detailed information on purchase transactions.

## Use Cases

For the Team:

**Target Audience**
- Leadership Role 1
- Leadership Role 2

**Example Scenario:** As a specific role, I want to ...

---

## Key Performance Indicators (KPIs)

The _Daily Purchase_ report includes the following KPIs:

- [**Purchase Quantity**](#purchase-quantity)  
- [**Purchase Amount**](#purchase-amount)  
- [**Cost Amount**](#cost-amount)  
- [**Gross Profit**](#gross-profit)  
- [**Gross Profit Margin**](#gross-profit-margin)

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

---
### Purchase Quantity

The *Purchase Quantity* is the total number of items sold within a specific time period.

**Formula**  

*Purchase Quantity* is the quantity of all value entries related to purchase for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Purchase Quantity*:
- Value Entry
- Purchase Line

---
### Purchase Amount

The *Purchase Amount* is the actual amount of items sold within a specific time period. This amount represents the net purchase amount in local currency, excluding VAT.

**Formula**  

*Purchase Amount* is the actual amount of all value entries related to purchase for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Purchase Amount*:
- Value Entry
- Purchase Line

---
### Cost Amount

The *Cost Amount* represents the total cost of goods sold incured by a location within a specific time period.

**Formula**  

*Cost Amount* is the the total cost of all purchase value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount*:
- Value Entry
- Purchase Line

---
### Gross Profit

The *Gross Profit* shows the difference between the purchase revenue and the cost of goods sold for a location within a specifict time period.

**Formula**  

*Gross Profit* = Purchase Amount - (Cost Amount + Cost Amount Non-Inv) 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry
- Purchase Line

---
### Gross Profit Margin

The *Gross Profit Margin* shows the gross profit as a percentage over the purchase amount.

**Formula**  

*Gross Profit Margin* = (Gross Profit / Purchase Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit Margin*:
- Value Entry
- Purchase Line


## Data used in the Daily Purchase report

Data from the following tables are used on the *Daily Purchase* report
- Value Entry
- Purchase Line
- Item


## See also
