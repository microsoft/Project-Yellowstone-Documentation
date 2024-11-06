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
- [Invoiced Amount](#invoiced-amount)
- [Invoiced Quantity)](#invoiced-quantity)
- [Outstanding Amount (Excl. VAT)](#outstanding-amount-excl-vat)
- [Outstanding Quantity](#outstanding-quantity)
- [Amt. Rcd. Not Invd. (Excl. VAT)](#amt-rcd-not-invd-excl-vat)
- [Quantity Rcd. Not Invd.](#amt-rcd-not-invd-excl-vat)


### No. of Distinct Items
**Formula**  
- This KPI calculates the number of unique items that have been purchased by counting the distinct values of the Item No. column of the Purchases table.

**Data Sources**
- Purchase Line
- Value Entry 

### No. of Outstanding Purchase Orders
**Formula**  
- This KPI calculates the number of unique purchase orders that are currently outstanding, by counting the distinct values of the Document No. column of the Purchases table, where Document Type = Order and Source Type = Purchase Order Outstanding.

**Data Sources**
- Purchase Line
- Value Entry

### No. of Purchase Invoices
**Formula**
- This KPI calculates the number of unique posted purchase invoices by countint the distinct count of the Document No. column from the Purchases table where Document Type = Purchase Invoice and Source Type = Value Entries Invoiced.

**Data Sources**
- Purchase Line
- Value Entry

### No. of Received Not Invd. Purchase Orders
**Formula**
- This KPI calculates the number of unique purchase orders that are received but not invoiced, by counting the distinct count of Document No. column from the Purchases table where Document Type = Order and Source Type = Purchase Orders Received Not Invoiced.

**Data Sources**
- Purchase Line
- Value Entry

### Invoiced Amount
**Formula**
- This KPI calculates the total amount of items that have been purchased and invoiced, by summing the Purchase Amount column of the Purchases table, where Source Type = Purchase Value Entries Invoiced.
- 
**Data Sources**
- Value Entry

### Invoiced Quantity
**Formula**
- This KPI calculates the total quantity of items that have been purchased and invoiced, by summing the Purchase Quantity column of the Purchases table, where Source Type = Purchase Value Entries Invoiced.

**Data Sources**
- Value Entry

### Outstanding Amount (Excl. VAT)
**Formula**  
- This KPI calculates the sum of Purchase Amount column from the Purchases table where Source Type = Purchase Order Outstanding, excluding VAT.

**Data Sources**
- Purchase Line

### Outstanding Quantity
**Formula**  
- This KPI calculates the sum of Purchase Qty. (Base) column from the Purchases table where Source Type = Purchase Order Outstanding.

**Data Sources**
- Purchase Line

### Amt. Rcd. Not Invd. (Excl. VAT)
**Formula**  
- This KPI calculates the sum of Purchase Amount column from the Purchases table where Source Type = Purchase Order Received Not Invoiced, excluding VAT.

**Data Sources**
- Purchase Line

### Quantity Rcd. Not Invd.
**Formula**  
- This KPI calculates the sum of Purchase Qty. (Base) column from the Purchases table. where Source Type = Purchase Order Received Not Invoiced.

**Data Sources**
- Purchase Line


## Purchase Budget Table
**Budget Measures**
- [Budget Amount](####)
- [Budget Amount Variance](####)
- [Budget Amount Variance %](####)
- [Budget Quantity](####)
- [Budget Quantity Variance](####)
- [Budget Quantity Variance %](####)

## Budget Amount
**Moving Annual Total Growth**
- [Budget Amount MAT (364)](####)
- [Budget Amount MAT (Fiscal)](####)
- [Budget Amount MATG (Fiscal)](####)
- [Budget Amount MATG % (Fiscal)](####)
- [Budget Amount PYMAT (Fiscal)](####)
- [Budget PYMAT (364)](####)

**Moving Averages**
- [Budget Amount AVG 1Y (Fiscal)](####)
- [Budget Amount AVG 30D (Fiscal)](####)
- [Budget Amount AVG 3M (Fiscal)](####)

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

## Budget Quantity
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

## Purchase Amount
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

## Purchase Quantity
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
