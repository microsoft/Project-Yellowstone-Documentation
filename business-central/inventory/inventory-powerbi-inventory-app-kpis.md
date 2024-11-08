---
title: Inventory KPIs and measures (Power BI)
description: The Inventory App KPIs provides a page to clearly identify all KPIs and Measures used in the Inventory Report.
author: kennienp
ms.author: kepontop
ms.reviewer: 
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 
ms.date: 11/08/2024
ms.service: dynamics-365-business-central
---

# Power BI Inventory app KPIs and measures

[!INCLUDE[applies-to-2024w2](includes/applies-to-2024w2.md)]

This page provides a list of all Key Performance Indicators (KPIs) included in the semantic model for the Power BI Purchases report. 

Explore the list of KPIs below to learn more about how they can help you achieve your business goals. 

Each KPI is described, including how it is calculated and what data was used in the calculations.

---
### Warehouse Quantity
**Formula**  
- This measure calculates the total quantity of an item that is currently in the warehouse by summing the base quantity from the Warehouse Entry table.

**Data Sources**
- Warehouse Entry

---
### Quantity in Adjustment Bin
**Formula**  
- This measure calculates the total quantity of an item that is currently in an adjustment bin by summing of the base quantity from the Warehouse Entry table only for the adjustment bins and filtering the Warehouse Entry table to only include entries for the adjustment bins.

**Data Sources**
- Warehouse Entry

---
### Available Qty. to Take
**Formula**  
- This measure calculates the quantity of an item that is available to be picked for sales or transfer orders. It subtracts the Pick Quantity (Base), ATO Components Pick Qty., and Negative Adjmt. Qty. (Base) measures from the Warehouse Quantity measure, but only for the bins that are not marked as adjustment bins. This gives you the total quantity of the item that is available to be picked for sales or transfer orders.

**Data Sources**
- Warehouse Entry
- Bin

---
### Pick Quantity (Base)
**Formula**  
- This measure calculates the total quantity of an item that has been picked from the warehouse for sales or transfer orders. It only includes the quantity that has been picked, not received or moved within the warehouse.

**Data Sources**
- Warehouse Activity Line

---
### ATO Components Pick Qty.
**Formula**  
- This measure calculates the total quantity of an item that has been taken from the warehouse specifically for assembling products that are made to order. It only includes the quantity that has been picked for assembling, not received or moved within the warehouse.

**Data Sources**
- Warehouse Activity Line

---
### Put-away Quantity (Base)
**Formula**  
- This measure calculates the total quantity of an item that has been placed in the warehouse for storage. It only includes the quantity that has been put away, not picked or moved within the warehouse.

**Data Sources**
- Warehouse Activity Line

### Negative Adjmt. Qty. (Base)
**Formula**  
- This measure calculates the total quantity of an item that has been removed from the warehouse due to adjustments. This includes any adjustments that result in inventory decreases in the Warehouse Journal Line table.

**Data Sources**
- Warehouse Journal Line

---
### Positive Adjmt. Qty. (Base)
**Formula**  
- This measure calculates the total quantity of an item that has been added to the warehouse due to adjustments. This includes any adjustments that result in inventory increases in the Warehouse Journal Line table.

**Data Sources**
- Warehouse Journal Line

---
### Gross Requirement
**Formula**  
- This measure calculates the total quantity of an item that is needed to fulfill various orders and projects. It includes the quantity that is on sales orders, service orders, projects, production order component lines, transaction order shipments, planning issues, assembly components, and purchased returns.

  *Gross Requirement = Qty. on Sales Order + Qty. on Service Order + Qty. on Projects + Qty. on Prod. Order Comp. Lines + Trans. Order Shipment (Qty.) + Planning Issues (Qty.) + Qty. on Asm. Component + Qty. on Purch. Return*

**Data Sources**
- Sales Line
- Purchase Line
- Transfer Line
- Service Line
- Job Planning Line
- Prod. Order Component
- Planning Component
- Assembly Line

---
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]


## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of inventory data](#TODO)   
[Built-in inventory reports](#TODO)   
[Inventory analytics overview](#TODO)  
[Inventory overview](#TODO)

[!INCLUDE[footer-include](includes/footer-banner.md)]
