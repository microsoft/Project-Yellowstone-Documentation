---
title: Scheduled Receipt (Power BI report)
description: The Scheduled Receipt gives users the ability to view inbound inventory into an organization broken up per document type. 
author: kennienp
ms.author: kepontop
ms.reviewer: 
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 37028_Primary
ms.date: 10/28/2024
ms.service: dynamics-365-business-central
---

# Scheduled Receipt (Power BI Report)
[!INCLUDE[applies-to-2024w2](includes/applies-to-2024w2.md)]


The *Scheduled Receipt* gives users the ability to view inbound inventory into an organization by different document types or processes. This is broken down by Item Cateogory or Item.

This also includes internal Assembly or Production accounting for when the finished good will become avaialble along with Purchase and Sales Return documents.

:::image type="content" source="media/inventory/scheduled-receipt.png" alt-text="Screenshot of the Scheduled Receipt Power BI Report" lightbox="media/inventory/scheduled-receipt.png":::

## How to use the report

This report is meant for managers and warehousing staff so they can easily identify when inventory will come in.

As a manager, you can use the *Scheduled Receipt* report to keep track of inventory levels and ensure that you are keeping up with the *Gross Requirement*(Add Link to Gross Requirement Report) by ensuring stock levels stay high. You can use this information to optimise your inventory manageament and ensure you aren't over buying or producing a specific item.

As a Warehouse Receipt working, this report is crucial in having detailed information of all inbound stock from both external and internal sources. This can assist in coordinating purchasing and production levels in future.

## Key Performance Indicators (KPIs)

The *Scheduled Receipt* report includes the following KPIs:

- [**Scheduled Receipt**](inventory-powerbi-kpis.md#scheduled-receipt)
- [**Projected Available Balance**](inventory-powerbi-kpis.md#projected-available-balance)
- [**FP Order Receipt (Qty.)**](inventory-powerbi-kpis.md#fp-order-receipt-qty)
- [**Rel. Order Receipt (Qty.)**](inventory-powerbi-kpis.md#rel-order-receipt-qty)
- [**Qty. On Purchase Order**](inventory-powerbi-kpis.md#qty-on-purch-order)
- [**Qty. in Transit**](inventory-powerbi-kpis.md#qty-in-transit)
- [**Trans. Order Receipt (Qty.)**](inventory-powerbi-kpis.md#trans-order-receipt-qty)
- [**Qty. on Assembly Order**](inventory-powerbi-kpis.md#qty-on-assembly-order)
- [**Qty. on Sales Return Order**](inventory-powerbi-kpis.md#qty-on-sales-return-order)

Click on the link for a KPI to learn more about what it means, how it is calculated, and what data was used in the calculations. 

[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]

## Data used in the report

Data from the following tables are used on the *Scheduled Receipt* report
- Item
- Purchase Line
- Sales Line
- Assembly Header
- Production Order Lines
- Transfer Lines

## Try the report

Try the report here: [Scheduled Receipt](https://businesscentral.dynamics.com?page=37028)

[!INCLUDE[ctrl-right-click-to-open-in-new-tab](includes/ctrl-right-click-to-open-in-new-tab.md)]

## See also
