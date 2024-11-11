---
title: Manufacturing KPIs and measures (Power BI)
description: Get an overview of all the KPIs and measures in the semantic model for the Manufacturing Power BI app.
author: kennienp
ms.author: kepontop
ms.reviewer:
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 
ms.date: 11/06/2024
ms.service: dynamics-365-business-central
---

# Power BI Manufacturing app KPIs and measures

[!INCLUDE[applies-to-2024w2](includes/applies-to-2024w2.md)]

This page provides a list of all Key Performance Indicators (KPIs) included in the semantic model for the Power BI Manufacturing report. 

Explore the list of KPIs below to learn more about how they can help you achieve your business goals. 

Each KPI is described, including how it is calculated and what data was used in the calculations.

## Production Data Table

**Capacity**
- [Load %](#load-)
- [Allocated Time (Hours)](#allocated-time-hours)
- [Capacity Available (Hours)](#capacity-available-hours)
- [Setup Time per Unit (Hours)](#setup-time-per-unit-hours)
- [Run Time per Unit (Hours)](#run-time-per-unit-hours)
- [Stop Time per Unit (Hours)](#stop-time-per-unit-hours)
- [Capacity Used per Unit (Hours)](#capacity-used-per-unit-hours)
- [Capacity Cost Amt. Deviation %](#capacity-cost-amt-deviation-)
- [Expected Capacity Cost Amount](#expected-capacity-cost-amount)
- [Capacity Cost Amt. (Actual)](#capacity-cost-amt-actual)
- [Capacity Cost Amt. Variance](#capacity-cost-amt-variance)
- [Capacity Used (Hours)](#capacity-used-hours)
- [Utilization %](#utilization-)
- [Expected Capacity Need (Hours)](#expected-capacity-need-hours)
- [Capacity Used Variance (Hours)](#capacity-used-variance-hours)
- [Capacity Scrap Qty.](#capacity-scrap-qty)

**Output**
- [Finished Quantity (Base)](#finished-quantity-base)
- [Expected Quantity (Base)](#expected-quantity-base)
- [Qty. Variance](#qty-variance)
- [Qty. Deviation %](#qty-deviation-)
- [Expected Cost Amt.](#expected-cost-amt)
- [Finished Cost Amt. (Actual)](#finished-cost-amt-actual)
- [Cost Amt. Variance](#cost-amt-variance)
- [Cost Amt. Deviation %](#cost-amt-deviation-)


**Consumption**
- [Consumption Cost Amt. Deviation %](#consumption-cost-amt-deviation-)
- [Expected Consumption Cost Amount](#expected-consumption-cost-amount)
- [Consumed Cost Amount (Actual)](#consumed-cost-amount-actual)
- [Consumption Cost Amt. Variance](#consumption-cost-amt-variance)

---
### Load %
**Formula**  
- This measure is calculates the percentage of available capacity that is currently being utilized, expressed as a percentage..
  
  *Load % = [Allocated Time (Hours)](#allocated-time-hours) / [Capacity Available (Hours)](#capacity-available-hours)*

**Data Sources**
- Calendar Entry
- Prod. Order Routing Line

---
### Allocated Time (Hours)
**Formula**  
- This measure shows the amount of time in hours that are allocated for production order routing lines by summing up all the allocated time values from the Production Data table.

**Data Sources**
- Prod. Order Capacity Need
- Prod. Order Routing Line

---
### Capacity Available (Hours)
**Formula**  
- This measure shows the total amount of available capacity in hours by summing up all capacity available values from the Production Data table.

**Data Sources**
- Calendar Entry

---
### Setup Time per Unit (Hours)
**Formula**  
- This measure shows the amount of time required to set up a machine or equipment for production.

  *Setup Time per Unit (Hours) = Setup Time (Hours) / [Finished Quantity (Base)](#finished-quantity-base)*

**Data Sources**
- Capacity Ledger Entry

---
### Run Time per Unit (Hours)
**Formula**  
- This measure is shows the amount of time required to produce a single unit of a product. 

  *Run Time per Unit (Hours) = Run Time (Hours) / [Finished Quantity (Base)](#finished-quantity-base)*

**Data Sources**
- Capacity Ledger Entry

---
### Stop Time per Unit (Hours)
**Formula**  
- This measure shows the amount of time lost due to equipment downtime or stoppages, per unit produced.

  *Stop Time per Unit (Hours) = Stop Time (Hours) / [Finished Quantity (Base)](#finished-quantity-base)*

**Data Sources**
- Capacity Ledger Entry

---
### Capacity Used per Unit (Hours)
**Formula**  
- This measure shows the amount of capacity utilized to produce a single unit of a product.

  *Capacity Used per Unit (Hours) = [Capacity Used (Hours)](#capacity-used-hours) / [Finished Quantity (Base)](#finished-quantity-base)*

**Data Sources**
- Capacity Ledger Entry

---
### Finished Quantity (Base)
**Formula**  
- This measure calculates the total quantity of finished products produced in base units over a given period by summing up all the output quantities from the Production Data table.

**Data Sources**
- Item Ledger Entry
- Location

---
### Capacity Cost Amt. Deviation %
**Formula**  
- This measure calculates the deviation between the actual capacity cost amount and the expected capacity cost amount, expressed as a percentage.

  *Capacity Cost Amt. Deviation % = ([Capacity Cost Amt. (Actual)](#capacity-cost-amt-actual) - [Expected Capacity Cost Amount](#expected-capacity-cost-amount))/ [Expected Capacity Cost Amount](#expected-capacity-cost-amount)*

**Data Sources**
- Item Ledger Entry
- Location

---
### Expected Capacity Cost Amount
**Formula**  
- This measure calculates the expected cost of capacity utilization for a given period by summing up the Expected Operation Cost Amount and the Expected Capacity Overhead Cost. The Expected Operation Cost Amount represents the expected cost of operating the equipment or machinery used in production, while the Expected Capacity Overhead Cost represents the expected cost of indirect resources used in production, such as rent, utilities, and maintenance.

  *Expected Capacity Cost Amount = Expected Operation Cost Amount + Expected Capacity Overhead Cost*

**Data Sources**
- Prod. Order Routing Line
- Location

---
### Capacity Cost Amt. (Actual)
**Formula**  
- This measure calculates the actual cost of capacity utilization for a given period bysumming up the Direct Cost and the Overhead Cost. The Direct Cost represents the direct expenses incurred in producing a product, while the Overhead Cost represents the indirect expenses incurred in producing a product, such as rent, utilities, and maintenance.

  *Capacity Cost Amt. (Actual) = Direct Cost + Overhead Cost*

**Data Sources**
- Capacity Ledger Entry

---
### Capacity Cost Amt. Variance
**Formula**  
- This measure calculates the variance between the expected cost of capacity utilization and the actual cost of capacity utilization.

  *Capacity Cost Amt. Variance = -([Expected Capacity Cost Amount](#expected-capacity-cost-amount) - [Capacity Cost Amt. (Actual)](#capacity-cost-amt-actual))*

**Data Sources**
- Capacity Ledger Entry
- Prod. Order Routing Line
- Location

---
### Consumption Cost Amt. Deviation %
**Formula**  
- This measure calculates the deviation between the actual consumption cost amount and the expected consumption cost amount, expressed as a percentage.

  *Consumption Cost Amt. Deviation % = ([Consumed Cost Amount (Actual)](#consumed-cost-amount-actual) - [Expected Consumption Cost Amount](#expected-consumption-cost-amount)) / [Expected Consumption Cost Amount](#expected-consumption-cost-amount)*

**Data Sources**
- Item Ledger Entry
- Location
- Prod. Order Component

---
### Expected Consumption Cost Amount
**Formula**  
- This measure shows the expected cost of consumed items for a given period by summing up the expected consumption cost of each item used in production. To calculate this cost amount, the measure multiplies the expected consumption quantity of each item by its related unit cost and then sums up the results from the Production Data table.

**Data Sources**
- Prod. Order Component

---
### Consumed Cost Amount (Actual)
**Formula**  
- This measure shows the actual cost of consumed items for a given period by summing up the actual cost of each item used in production. To calculate this cost amount, the measure calculates the sum of the actual cost of items consumed from the Production Data Table, filtered for the Consumption data source.

**Data Sources**
- Item Ledger Entry
- Location

---
### Consumption Cost Amt. Variance
**Formula**  
- This measure shows the variance between the expected cost of consumed items and the actual cost of consumed items. 

  *Consumption Cost Amt. Variance = -([Expected Consumption Cost Amount](#expected-consumption-cost-amount) - [Consumed Cost Amount (Actual)](#consumed-cost-amount-actual))*

**Data Sources**
- Prod. Order Component
- Item Ledger Entry
- Location

---
### Capacity Used (Hours)
**Formula**  
- This measure shows the total number of capacity hours used by summing up the capacity requirement for each production activity from the Production Data table.

**Data Sources**
- Capacity Ledger Entry

---
### Utilization %
**Formula**  
- This measure shows the percentage of available capacity that was utilized.

  *Utilization % = ([Capacity Used (Hours)](#capacity-used-hours) / [Capacity Available (Hours)](#capacity-available-hours)*

**Data Sources**
- Capacity Ledger Entry
- Calendar Entry

---
### Expected Capacity Need (Hours)
**Formula**  
- This measure shows the expected total capacity required for production by summing up the expected capacity need (in hours) for each production activity from the Production Data table.

**Data Sources**
- Prod. Order Routing Line

---
### Capacity Used Variance (Hours)
**Formula**  
- This measure shows the variance between the expected capacity need and the actual capacity used.

  *Capacity Used Variance (Hours) = -([Expected Capacity Need (Hours)](#expected-capacity-need-hours) - [Capacity Used (Hours)](#capacity-used-hours))*

**Data Sources**
- Prod. Order Routing Line
- Capacity Ledger Entry

---
### Expected Quantity (Base)
**Formula**  
- This measure calculates the total expected quantity (in base units) for a given period by summing up the base quantity for each production order line from the Production Data table.

**Data Sources**
- Prod. Order Line
- Location

---
### Qty. Variance
**Formula**  
- This measure calculates the variance between the expected quantity and the actual quantity produced.
  
**Data Sources**
- Item Ledger Entry
- Prod. Order Line
- Location

---
### Qty. Deviation %
**Formula**  
- This measure shows the deviation between the expected quantity and the actual quantity produced, expressed as a percentage.

  *Qty. Deviation % = ([Finished Quantity (Base)](#finished-quantity-base) - [Expected Quantity (Base)](#expected-quantity-base)) / [[Expected Quantity (Base)](#expected-quantity-base)*
  
**Data Sources**
- Item Ledger Entry
- Prod. Order Line
- Location

---
### Expected Cost Amt.
**Formula**  
- This measure shows the total expected cost amount by multiplying the quantity (in base units) for each production order line from the Production Data Table by the unit cost (in local currency) for the corresponding item, and summing up the results.
  
**Data Sources**
- Prod. Order Line
- Location


---
### Finished Cost Amt. (Actual)
**Formula**  
- This measure shows total actual cost amount for finished goods produced by summing up the actual cost amount for each output item ledger entry from the Production Data Table.
  
**Data Sources**
- Item Ledger Entry
- Location

---
### Cost Amt. Variance
**Formula**  
- This measure calculates the variance between the expected cost amount and the actual cost amount for finished goods produced.

  *Cost Amt. Variance = -([Expected Cost Amt.](#expected-cost-amt) - [Finished Cost Amt. (Actual)](#finished-cost-amt-actual))*
  
**Data Sources**
- Item Ledger Entry
- Prod. Order Line
- Location

---
### Cost Amt. Deviation %
**Formula**  
- This measure calculates the deviation between the expected cost amount and the actual cost amount for finished goods produced, expressed as a percentage.

  *Cost Amt. Deviation % = ([Finished Cost Amt. (Actual)](#finished-cost-amt-actual) - [Expected Cost Amt.](#expected-cost-amt)) / [Expected Cost Amt.](#expected-cost-amt)*
  
**Data Sources**
- Item Ledger Entry
- Prod. Order Line
- Location

---
### Capacity Scrap Qty.
**Formula**  
- This measure calculates the total scrap quantity in a given period by summing up the scrap quantity for each capacity ledger entry from the Production Data table.
  
**Data Sources**
- Capacity Ledger Entry


---
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]


## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of manufacturing data](#TODO)   
[Built-in purchasing reports](#TODO)   
[Manufacturing analytics overview](#TODO)  
[Manufacturing overview](#TODO)

[!INCLUDE[footer-include](includes/footer-banner.md)]
