---
title: Purchases KPIs and measures (Power BI)
description: Get an overview of all the KPIs and measures in the semantic model for the Purchases Power BI app.
author: kennienp
ms.author: kepontop
ms.reviewer:
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 
ms.date: 11/06/2024
ms.service: dynamics-365-business-central
---

# Power BI Purchases app KPIs and measures

[!INCLUDE[applies-to-2024w2](includes/applies-to-2024w2.md)]

This page provides a list of all Key Performance Indicators (KPIs) included in the semantic model for the Power BI Purchases report. 

Explore the list of KPIs below to learn more about how they can help you achieve your business goals. 

Each KPI is described, including how it is calculated and what data was used in the calculations.

## Purchases Table
**Purchase Measures**
- [No. of Distinct Items](#no-of-distinct-items)
- [No. of Outstanding Purchase Orders](#no-of-outstanding-purchase-orders)
- [No. of Purchase Invoices](#no-of-purchase-invoices)
- [No. of Received Not Invd. Purchase Orders](#no-of-received-not-invd-purchase-orders)
- [Purchase Amount](#invoiced-amount)
- [Purchase Quantity)](#invoiced-quantity)
- [Invoiced Amount](#invoiced-amount)
- [Invoiced Quantity)](#invoiced-quantity)
- [Outstanding Amount (Excl. VAT)](#outstanding-amount-excl-vat)
- [Outstanding Quantity](#outstanding-quantity)
- [Amt. Rcd. Not Invd. (Excl. VAT)](#amt-rcd-not-invd-excl-vat)
- [Quantity Rcd. Not Invd.](#amt-rcd-not-invd-excl-vat)

---
### No. of Distinct Items
**Formula**  
- This KPI calculates the number of unique items that have been purchased by counting the distinct values of the Item No. column of the Purchases table.

**Data Sources**
- Purchase Line
- Value Entry 

---
### No. of Outstanding Purchase Orders
**Formula**  
- This KPI calculates the number of unique purchase orders that are currently outstanding, by counting the distinct values of the Document No. column of the Purchases table, where Document Type = Order and Source Type = Purchase Order Outstanding.

**Data Sources**
- Purchase Line
- Value Entry

---
### No. of Purchase Invoices
**Formula**
- This KPI calculates the number of unique posted purchase invoices by countint the distinct count of the Document No. column from the Purchases table where Document Type = Purchase Invoice and Source Type = Value Entries Invoiced.

**Data Sources**
- Purchase Line
- Value Entry

---
### No. of Received Not Invd. Purchase Orders
**Formula**
- This KPI calculates the number of unique purchase orders that are received but not invoiced, by counting the distinct count of Document No. column from the Purchases table where Document Type = Order and Source Type = Purchase Orders Received Not Invoiced.

**Data Sources**
- Purchase Line
- Value Entry

---
### Purchase Amount
**Formula**
- This KPI sums the the Purchase Amount column of the Purchases table.

**Data Sources**
- Value Entry

---
### Purchase Quantity
**Formula**
- This KPI sums the the Purchase Quantity column of the Purchases table.

**Data Sources**
- Value Entry

---
### Invoiced Amount
**Formula**
- This KPI calculates the total amount of items that have been purchased and invoiced, by summing the Purchase Amount column of the Purchases table, where Source Type = Purchase Value Entries Invoiced.
- 
**Data Sources**
- Value Entry

---
### Invoiced Quantity
**Formula**
- This KPI calculates the total quantity of items that have been purchased and invoiced, by summing the Purchase Quantity column of the Purchases table, where Source Type = Purchase Value Entries Invoiced.

**Data Sources**
- Value Entry

---
### Outstanding Amount (Excl. VAT)
**Formula**  
- This KPI calculates the sum of Purchase Amount column from the Purchases table where Source Type = Purchase Order Outstanding, excluding VAT.

**Data Sources**
- Purchase Line

---
### Outstanding Quantity
**Formula**  
- This KPI calculates the sum of Purchase Qty. (Base) column from the Purchases table where Source Type = Purchase Order Outstanding.

**Data Sources**
- Purchase Line

---
### Amt. Rcd. Not Invd. (Excl. VAT)
**Formula**  
- This KPI calculates the sum of Purchase Amount column from the Purchases table where Source Type = Purchase Order Received Not Invoiced, excluding VAT.

**Data Sources**
- Purchase Line

---
### Quantity Rcd. Not Invd.
**Formula**  
- This KPI calculates the sum of Purchase Qty. (Base) column from the Purchases table. where Source Type = Purchase Order Received Not Invoiced.

**Data Sources**
- Purchase Line


## Purchase Budget Table
**Budget Measures**
- [Budget Amount](#budget-amount)
- [Budget Amount Variance](#budget-amount-variance)
- [Budget Amount Variance %](#budget-amount-variance-)
- [Budget Quantity](#budget-quantity)
- [Budget Quantity Variance](#budget-quantity-variance)
- [Budget Quantity Variance %](#budget-quantity-variance-)

**Moving Annual Total Growth**
- [Budget Amount MAT (Fiscal)](####)
- [Budget Amount MATG (Fiscal)](####)
- [Budget Amount MATG % (Fiscal)](####)
- [Budget Amount PYMAT (Fiscal)](####)

**Moving Averages**
- [Budget Amount AVG 1Y (Fiscal)](####)
- [Budget Amount AVG 30D (Fiscal)](####)
- [Budget Amount AVG 3M (Fiscal)](####)

---
### Budget Amount
**Formula**  
- This KPI calculates the sum of Purchase Amount column from the Purchase Budget table.

**Data Sources**
- Item Budget Entries

---
### Budget Amount Variance
**Formula**
- *Budget Amount Variance = Purchase Amount - Budget Amount*

**Data Sources**
- Item Budget Entry
- Purchase Line
- Value Entry

---
### Budget Amount Variance %
**Formula**  
- *Budget Amount Variance % = Budget Amount Variance - Budget Amount*

**Data Sources**
- Item Budget Entry
- Purchase Line
- Value Entry

---
### Budget Quantity
**Formula**  
- This KPI sums the Quantity column from the Purchase Budget table.

**Data Sources**
- Item Budget Entry

---
### Budget Quantity Variance
**Formula**  
- *Budget Quantity Variance = Purchase Quantity - Budget Quantity*

**Data Sources**
- Item Budget Entry
- Purchase Line
- Value Entry

---
### Budget Quantity Variance %
**Formula**  
- *Budget Quantity Variance % = Budget Quantity Variance - Budget Quantity*

**Data Sources**
- Item Budget Entry
- Purchase Line
- Value Entry

---
### Budget Amount MAT (Fiscal)
**Formula**  
- This measure calculates the purchases for the last 12 months (moving annual total) using the fiscal calendar by summing up the purchases between the calculated first and last days of the 365-day period.

**Data Sources**
- Value Entry
- Purchase Line
- Date (Fiscal Calendar)

---
### Budget Amount MATG (Fiscal)
**Formula**  
- This measure compares the current period's moving annual total purchases to the previous period's moving annual total purchases. If both values are not blank, it subtracts the previous period's purchases from the current period's purchases to determine the growth. The result is returned, representing the change in purchases between the two periods.

**Data Sources**
- Value Entry
- Purchase Line
- Date (Fiscal Calendar)

---
### Budget Amount MATG % (Fiscal)
**Formula**  
- *Budget Amount MATG % (Fiscal) = Budget Amount MATG (Fiscal) / Budget Amount PYMAT x 100* 

**Data Sources**
- Value Entry
- Purchase Line
- Date (Fiscal Calendar)

---
### Budget Amount PYMAT (Fiscal)
**Formula**  
- This measure calculates the previous year moving annual total (PYMAT) of the Budget Amount by subtracting one year from the current date.

**Data Sources**
- Value Entry
- Purchase Line
- Date (Fiscal Calendar)

---
### Budget Amount AVG 1Y (Fiscal)
**Formula**  
- This measure calculates the average budet amount for the past year.
  
**Data Sources**
- Value Entry
- Purchase Line
- Date (Fiscal Calendar)

---
### Budget Amount AVG 30D (Fiscal)
**Formula**  
- This measure calculates the average budet amount for the past 30 days.
  
**Data Sources**
- Value Entry
- Purchase Line
- Date (Fiscal Calendar)

---
### Budget Amount AVG 3M (Fiscal)
**Formula**  
- This measure calculates the average budet amount for the past 3 months.
  
**Data Sources**
- Value Entry
- Purchase Line
- Date (Fiscal Calendar)

## Purchase Budget Table - Budget Amount
**Period-over-Period Growth**
- [Budget Amount MOM (Fiscal)](####)
- [Budget Amount MOM % (Fiscal)](####)
- [Budget Amount PM (Fiscal)](####)
- [Budget Amount POP (Fiscal)](####)
- [Budget Amount POP % (Fiscal)](####)
- [Budget Amount PP (Fiscal)](####)
- [Budget Amount PQ (Fiscal)](####)
- [Budget Amount PY (Fiscal)](####)
- [Budget Amount QOQ (Fiscal)](####)
- [Budget Amount QOQ % (Fiscal)](####)
- [Budget Amount YOY (Fiscal)](####)
- [Budget Amount YOY% (Fiscal)](####)

**Period-to-Date Growth**
- [Budget Amount MOMTD (Fiscal)](####)
- [Budget Amount MOMTD % (Fiscal)](####)
- [Budget Amount PMTD (Fiscal)](####)
- [Budget Amount PQTD (Fiscal)](####)
- [Budget Amount PYTD (Fiscal)](####)
- [Budget Amount QOQTD (Fiscal)](####)
- [Budget Amount QOQTD % (Fiscal)](####)
- [Budget Amount YOYTD (Fiscal)](####)
- [Budget Amount YOYTD % (Fiscal)](####)

**Period-to-Date Over Full Previous Period**
- [Budget Amount MTDOPM (Fiscal)](####)
- [Budget Amount MTDOPM % (Fiscal)](####)
- [Budget Amount PMC (Fiscal)](####)
- [Budget Amount PQC (Fiscal)](####)
- [Budget Amount PYC (Fiscal)](####)
- [Budget Amount QTDOPQ (Fiscal)](####)
- [Budget Amount QTDOPQ % (Fiscal)](####)
- [Budget Amount YTDOPY (Fiscal)](####)
- [Budget Amount YTDOPY % (Fiscal)](####)

**Period-to-Date Total**
- [Budget Amount MTD (Fiscal)](####)
- [Budget Amount QTD (Fiscal)](####)
- [Budget Amount YTD (Fiscal)](####)

## Purchase Budget Table - Budget Quantity
**Moving Annual Total Growth**
- [Budget Quantity MAT (364)](####)
- [Budget Quantity MATG (Fiscal)](####)
- [Budget Quantity MATG % (Fiscal)](####)
- [Budget Quantity PYMAT (Fiscal)](####)

**Moving Averages**
- [Budget Quantity AVG 1Y (Fiscal)](####)
- [Budget Quantity AVG 30D (Fiscal)](####)
- [Budget Quantity AVG 3M (Fiscal)](####)

**Period-over-Period Growth**
- [Budget Quantity MOM (Fiscal)](####)
- [Budget Quantity MOM % (Fiscal)](####)
- [Budget Quantity PM (Fiscal)](####)
- [Budget Quantity POP (Fiscal)](####)
- [Budget Quantity POP % (Fiscal)](####)
- [Budget Quantity PP (Fiscal)](####)
- [Budget Quantity PQ (Fiscal)](####)
- [Budget Quantity PY (Fiscal)](####)
- [Budget Quantity QOQ (Fiscal)](####)
- [Budget Quantity QOQ % (Fiscal)](####)
- [Budget Quantity YOY (Fiscal)](####)
- [Budget Quantity YOY % (Fiscal)](####)

**Period-to-Date Growth**
- [Budget Quantity MOMTD (Fiscal)](####)
- [Budget Quantity MOMTD % (Fiscal)](####)
- [Budget Quantity PMTD (Fiscal)](####)
- [Budget Quantity PQTD (Fiscal)](####)
- [Budget Quantity PYTD (Fiscal)](####)
- [Budget Quantity QOQTD (Fiscal)](####)
- [Budget Quantity QOQTD % (Fiscal)](####)
- [Budget Quantity YOYTD (Fiscal)](####)
- [Budget Quantity YOYTD % (Fiscal)](####)

**Period-to-Date Over Full Previous Period**
- [Budget Quantity MTDOPM (Fiscal)](####)
- [Budget Quantity MTDOPM % (Fiscal)](####)
- [Budget Quantity PMC (Fiscal)](####)
- [Budget Quantity PQC (Fiscal)](####)
- [Budget Quantity PYC (Fiscal)](####)
- [Budget Quantity QTDOPQ (Fiscal)](####)
- [Budget Quantity QTDOPQ % (Fiscal)](####)
- [Budget Quantity YTDOPY (Fiscal)](####)
- [Budget Quantity YTDOPY % (Fiscal)](####)

**Period-to-Date Total**
- [Budget Quantity MTD (Fiscal)](####)
- [Budget Quantity QTD (Fiscal)](####)
- [Budget Quantity YTD (Fiscal)](####)

## Purchases Table - Purchase Amount
**Moving Annual Total Growth**
- [Purchase Amount MAT (364)](####)
- [Purchase Amount MAT](####)
- [Purchase Amount MATG (Fiscal)](####)
- [Purchase Amount MATG % (Fiscal)](####)
- [Purchase Amount PYMAT (Fiscal)](####)
- [Purchase PYMAT)](####)

**Moving Averages**
- [Purchase Amount AVG 1Y (Fiscal)](####)
- [Purchase Amount AVG 30D (Fiscal)](####)
- [Purchase Amount AVG 3M (Fiscal)](####)

**Period-over-Period Growth**
- [Purchase Amount MOM (Fiscal)](####)
- [Purchase Amount MOM % (Fiscal)](####)
- [Purchase Amount PM (Fiscal)](####)
- [Purchase Amount POP (Fiscal)](####)
- [Purchase Amount POP % (Fiscal)](####)
- [Purchase Amount PP (Fiscal)](####)
- [Purchase Amount PQ (Fiscal)](####)
- [Purchase Amount PY (Fiscal)](####)
- [Purchase Amount QOQ (Fiscal)](####)
- [Purchase Amount QOQ % (Fiscal)](####)
- [Purchase Amount YOY (Fiscal)](####)
- [Purchase Amount YOY % (Fiscal)](####)

**Period-to-Date Growth**
- [Purchase Amount MOMTD (Fiscal)](####)
- [Purchase Amount MOMTD % (Fiscal)](####)
- [Purchase Amount PMTD (Fiscal)](####)
- [Purchase Amount PQTD (Fiscal)](####)
- [Purchase Amount PYTD (Fiscal)](####)
- [Purchase Amount QOQTD (Fiscal)](####)
- [Purchase Amount QOQTD % (Fiscal)](####)
- [Purchase Amount YOYTD (Fiscal)](####)
- [Purchase Amount YOYTD % (Fiscal)](####)

**Period-to-Date Over Full Previous Period**
- [Purchase Amount MTDOPM (Fiscal)](####)
- [Purchase Amount MTDOPM % (Fiscal)](####)
- [Purchase Amount PMC (Fiscal)](####)
- [Purchase Amount PQC (Fiscal)](####)
- [Purchase Amount PYC (Fiscal)](####)
- [Purchase Amount QTDOPQ (Fiscal)](####)
- [Purchase Amount QTDOPQ % (Fiscal)](####)
- [Purchase Amount YTDOPY (Fiscal)](####)
- [Purchase Amount YTDOPY % (Fiscal)](####)

**Period-to-Date Total**
- [Purchase Amount MTD (Fiscal)](####)
- [Purchase Amount QTD (Fiscal)](####)
- [Purchase Amount YTD (Fiscal)](####)

## Purchases Table - Purchase Quantity
**Moving Annual Total Growth**
- [Purchase Quantity MAT (Fiscal)](####)
- [Purchase Quantity MATG (Fiscal)](####)
- [Purchase Quantity MATG % (Fiscal)](####)
- [Purchase Quantity PYMAT (Fiscal)](####)

**Moving Averages**
- [Purchase Quantity AVG 1Y (Fiscal)](####)
- [Purchase Quantity AVG 30D (Fiscal)](####)
- [Purchase Quantity AVG 3M (Fiscal)](####)

**Period-over-Period Growth**
- [Purchase Quantity MOM (Fiscal)](####)
- [Purchase Quantity MOM % (Fiscal)](####)
- [Purchase Quantity PM (Fiscal)](####)
- [Purchase Quantity POP (Fiscal)](####)
- [Purchase Quantity POP % (Fiscal)](####)
- [Purchase Quantity PP (Fiscal)](####)
- [Purchase Quantity PQ (Fiscal)](####)
- [Purchase Quantity PY (Fiscal)](####)
- [Purchase Quantity QOQ (Fiscal)](####)
- [Purchase Quantity QOQ % (Fiscal)](####)
- [Purchase Quantity YOY (Fiscal)](####)
- [Purchase Quantity YOY % (Fiscal)](####)

**Period-to-Date Growth**
- [Purchase Quantity MOMTD (Fiscal)](####)
- [Purchase Quantity MOMTD % (Fiscal)](####)
- [Purchase Quantity PMTD (Fiscal)](####)
- [Purchase Quantity PQTD (Fiscal)](####)
- [Purchase Quantity PYTD (Fiscal)](####)
- [Purchase Quantity QOQTD (Fiscal)](####)
- [Purchase Quantity QOQTD % (Fiscal)](####)
- [Purchase Quantity YOYTD (Fiscal)](####)
- [Purchase Quantity YOYTD % (Fiscal)](####)

**Period-to-Date Over Full Previous Period**
- [Purchase Quantity MTDOPM (Fiscal)](####)
- [Purchase Quantity MTDOPM % (Fiscal)](####)
- [Purchase Quantity PMC (Fiscal)](####)
- [Purchase Quantity PQC (Fiscal)](####)
- [Purchase Quantity PYC (Fiscal)](####)
- [Purchase Quantity QTDOPQ (Fiscal)](####)
- [Purchase Quantity QTDOPQ % (Fiscal)](####)
- [Purchase Quantity YTDOPY (Fiscal)](####)
- [Purchase Quantity YTDOPY % (Fiscal)](####)

**Period-to-Date Total**
- [Purchase Quantity MTD (Fiscal)](####)
- [Purchase Quantity QTD (Fiscal)](####)
- [Purchase Quantity YTD (Fiscal)](####)

---
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]


## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of purchasing data](#TODO)   
[Built-in purchasing reports](#TODO)   
[Purchasing analytics overview](#TODO)  
[Purchases overview](#TODO)

[!INCLUDE[footer-include](includes/footer-banner.md)]