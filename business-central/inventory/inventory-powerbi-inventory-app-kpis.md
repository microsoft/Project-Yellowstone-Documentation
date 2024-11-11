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

This page provides a list of all Key Performance Indicators (KPIs) included in the semantic model for the Power BI Inventory report. 

Explore the list of KPIs below to learn more about how they can help you achieve your business goals. 

Each KPI is described, including how it is calculated and what data was used in the calculations.

## Bins Table
- [Warehouse Quantity](#warehouse-quantity)  
- [Quantity in Adjustment Bin](#quantity-in-adjustment-bin)  
- [Available Qty. to Take](#available-qty-to-take)  
- [Pick Quantity (Base)](#pick-quantity-base)  
- [ATO Components Pick Qty.](#ato-components-pick-qty)  
- [Put-away Quantity (Base)](#put-away-quantity-base)  
- [Negative Adjmt. Qty. (Base)](#negative-adjmt-qty-base)  
- [Positive Adjmt. Qty. (Base)](#positive-adjmt-qty-base)  

## Items Table
- [Gross Requirement](#gross-requirement)  
- [Projected Available Balance](#projected-available-balance)
- [Scheduled Receipt](#scheduled-receipt)
- [Planned Order Receipt](#planned-order-receipt)  
- [Planned Order Releases](#planned-order-releases)  


## Sales Lines Table
- [Qty. on Sales Order](#qty-on-sales-order)
- [Qty. on Sales Return Order](#qty-on-sales-return-order)  


## Purchase Lines Table
- [Qty. on Purch. Order](#qty-on-purch-order)  
- [Qty. on Purch. Return](#qty-on-purch-return)

## Service Lines Table
- [Qty. on Service Order](#qty-on-service-order)  

## Project Planning Lines Table
- [Qty. on Projects](#qty-on-projects)

## Prod. Order Component Lines Table
- [Qty. on Prod. Order](#qty-on-prod-order)
- [Qty. on Prod. Order Comp. Lines](#qty-on-prod-order-comp-lines)  

## Transfer Lines Table
- [Qty. in Transit](#qty-in-transit)  
- [Trans. Order Shipment (Qty.)](#trans-order-shipment-qty)
- [Trans. Order Receipt (Qty.)](#trans-order-receipt-qty)
- [Trans. Order Shipment (Qty.)](#trans-order-shipment-qty-1)  


## Planning Component Lines Table
- [Planning Issues (Qty.)](#planning-issues-qty)  

## Assembly Headers Table
- [Qty. on Assembly Order](#qty-on-assembly-order)

## Assembly Lines Table
- [Qty. on Asm. Component](#qty-on-asm-component)  

## Production Order Lines Table
- [FP Order Receipt (Qty.)](#fp-order-receipt-qty)  
- [Rel. Order Receipt (Qty.)](#rel-order-receipt-qty)

## Item Ledger Entries Table
- [Quantity](#quantity)  
- [Inventory (Quantity)](#inventory-quantity)  
- [Expired Inventory](#expired-inventory) 
- [Net Qty. Purchased](#net-qty-purchased)  
- [Net Qty. Sold](#net-qty-sold)

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
### Projected Available Balance
**Formula**  
- This measure calculates the current inventory quantity, planned order receipts, scheduled receipts, and gross requirements based on the data up until the most recent date available.

  *Projected Available Balance = Inventory (Quantity) + Planned Order Receipt + Scheduled Receipt - Gross Requirement*

**Data Sources**
- Sales Line
- Purchase Line
- Transfer Line
- Service Line
- Job Planning Line
- Prod. Order Component
- Planning Component
- Assembly Line
- Item Ledger Entry
- Requisition Line
- Production Order Line

---
### Qty. on Sales Order
**Formula**  
- This measure shows how many items have been ordered by customers but are yet to be delivered or shipped by summing up the total outstanding quantity of items on all sales order lines. 

**Data Sources**
- Sales Line

---
### Qty. on Purch. Return
**Formula**  
- This measure shows how many items have been returned to the supplier but are yet to be received or credited by summing up the total outstanding quantity of items on all purchase return order lines.

**Data Sources**
- Purchase Line

---
### Qty. on Service Order
**Formula**  
- This measure represents how many service items or hours have been ordered by customers but are yet to be fulfilled by summing up the total outstanding quantity of items or hours on all service order lines.

**Data Sources**
- Service Line

---
### Qty. on Projects
**Formula**  
- This measure shows how many items or hours are yet to be completed on a project by summing up the total outstanding quantity of items or hours on all project lines.

**Data Sources**
- Job Planning Line

---
### Qty. on Prod. Order Comp. Lines
**Formula**  
- This measure shows how many items are yet to be completed on a production order by summing up the total remaining quantity of items on all production order component lines.

**Data Sources**
- Prod. Order Component

---
### Trans. Order Shipment (Qty.)
**Formula**  
- This measure shows how many items have been shipped between two locations by summing up the total outstanding quantity of items on all transfer order lines that are associated with the specified location codes and shipment date.

**Data Sources**
- Location
- Transfer Line

---
### Planning Issues (Qty.)
**Formula**  
- This measure shows how many items are expected to be consumed for planned production orders by summing up the expected quantity of items that are required for production.

**Data Sources**
- Planning Component

---
### Qty. on Asm. Component
**Formula**  
- This measure shows how many items are yet to be assembled for a finished product by summing up the remaining quantity of items on all assembly lines.

**Data Sources**
- Assembly Line

---
### Qty. on Purch. Order
**Formula**  
- This measure shows how many items are yet to be received for purchase orders by summing up the outstanding quantity of items on all purchase order lines.

**Data Sources**
- Purchase Line

---
### Qty. in Transit
**Formula**  
- This measure shows how many items are currently in transit between locations by summing up the quantity of items in transit on all transfer lines.

**Data Sources**
- Location
- Transfer Line

---
### FP Order Receipt (Qty.)
**Formula**  
- This measure is abbreviated for Firmed Planned Order Receipt (Qty.) and hows how many items are expected to be received for firm planned production orders by summing up the remaining quantity of items on all firm planned production order lines.

**Data Sources**
- Production Order Line

---
### Rel. Order Receipt (Qty.)
**Formula**  
- This measure is abbreviated for Released Production Order Receipt (Qty.) and shows how many items are expected to be received for released production orders by summing up the remaining quantity of items on all released production order lines.

**Data Sources**
- Production Order Line

---
### Trans. Order Receipt (Qty.)
**Formula**  
- This measure shows how many items are expected to be received for transfer orders by summing up the outstanding quantity of items on all transfer lines.

**Data Sources**
- Location
- Transfer Line

---
### Qty. on Assembly Order
**Formula**  
- This measure shows how many items are yet to be assembled for assembly orders by summing up the remaining quantity of items on all assembly headers.

**Data Sources**
- Assembly Header

---
### Trans. Order Shipment (Qty.)
**Formula**  
- This measure shows how many items are expected to be shipped for transfer orders by summing up the outstanding quantity of items on all transfer lines that are yet to be shipped from the source location.

**Data Sources**
- Location
- Transfer Line

---
### Inventory (Quantity)
**Formula**  
- This measure shows the total quantity of inventory on hand for all items by summing up the quantity of items on all item ledger entries.

**Data Sources**
- Item Ledger Entry

---
### Qty. on Prod. Order
**Formula**  
- This measure shows how many items are yet to be produced for production orders by summing up the remaining quantity of items on all planned, firm planned, and released production order lines.

**Data Sources**
- Production Order Line

---
### Qty. on Sales Return Order
**Formula**  
- This measure shows how many items are yet to be returned by customers for sales return orders by summing up the outstanding quantity of items on all sales lines that are associated with return orders.

**Data Sources**
- Production Order Line

---
### Quantity
**Formula**  
- This measure shows the total quantity of items that have been processed through the item ledger by summing up the quantity of items on all item ledger entries including sales, purchases, adjustments, and other types of transactions.

**Data Sources**
- Item Ledger Entry

---
### Expired Inventory
**Formula**  
- This measure shows how much inventory has expired and is no longer available for sale or use by calculating the remaining quantity of items on all item ledger entries.

**Data Sources**
- Item Ledger Entry

---
### Scheduled Receipt
**Formula**  
- This measure shows the total quantity of items that are scheduled to be received by the company.

  *Scheduled Receipt = FP Order Receipt (Qty.) + Rel. Order Receipt (Qty.) + Qty. on Purch. Order + Qty. in Transit + Trans. Order Receipt (Qty.) + Qty. on Assembly Order + Qty. on Sales Return Order*

**Data Sources**
- Sales Line
- Purchase Line
- Transfer Line
- Assembly Header
- Production Order Line

---
### Planned Order Receipt
**Formula**  
- This measure shows the total quantity of items that are planned to be received by the company through planned orders and purchase requisitions.

  *Planned Order Receipt = Planned Order Receipt (Qty.) + Purch. Req. Receipt (Qty.)*

**Data Sources**
- Production Order Line
- Requisition Line

---
### Planned Order Releases
**Formula**  
- This measure shows the total quantity of items that are planned to be released through planned orders and purchase requisitions.

  *Planned Order Releases = Planned Order Release (Qty.) + Purch. Req. Release (Qty.)*

**Data Sources**
- Production Order Line
- Requisition Line

---
###  Net Qty. Purchased
**Formula**  
- This measure shows the total quantity of items that have been purchased and received by the company by calculating the quantity, filtered to only include item ledger entries that have an entry type of "Purchase".

**Data Sources**
- Item Ledger Entry

---
###  Net Qty. Sold
**Formula**  
- This measure shows the total quantity of items that have been sold by the company by calculating the quantity, filtered to only include item ledger entries that have an entry type of "Sale".

**Data Sources**
- Item Ledger Entry

---
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]


## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of inventory data](#TODO)   
[Built-in inventory reports](#TODO)   
[Inventory analytics overview](#TODO)  
[Inventory overview](#TODO)

[!INCLUDE[footer-include](includes/footer-banner.md)]
