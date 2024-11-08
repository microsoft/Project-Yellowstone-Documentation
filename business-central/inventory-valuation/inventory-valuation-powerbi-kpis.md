---
title: Inventory Valuation KPIs and measures (Power BI)
description: The Inventory Valuation App KPIs provides a page to clearly identify all KPIs and Measures used in the Inventory Valuation Report.
author: kennienp
ms.author: kepontop
ms.reviewer: 
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 
ms.date: 11/08/2024
ms.service: dynamics-365-business-central
---

# Power BI Inventory Valuation app KPIs and measures

[!INCLUDE[applies-to-2024w2](includes/applies-to-2024w2.md)]

This page provides a list of all Key Performance Indicators (KPIs) included in the semantic model for the Power BI Purchases report. 

Explore the list of KPIs below to learn more about how they can help you achieve your business goals. 

Each KPI is described, including how it is calculated and what data was used in the calculations.

## Value Entries Table   
- [Ending Balance Qty.](#ending-balance-qty)  
- [Increases Value](#increases-value)  
- [Decreases Value](#decreases-value)  
- [Beginning Balance Value](#beginning-balance-value)  
- [Ending Balance Value](#ending-balance-value)  
- [Ending Balance Posted to G/L](#ending-balance-posted-to-gl)  
- [Variance](#variance)  
- [Invoiced Quantity](#invoiced-quantity)  
- [Increases Qty](#increases-qty)  
- [Decreases Qty](#decreases-qty)

---
### Ending Balance Qty.
**Formula**  
- This measure calculates the total quantity of items remaining at the end of a specific period.

  *Ending Balance Qty. = Beginning Balance Qty. + Net Balance Qty.*

**Data Sources**
- Value Entry 

---
### Increases Value
**Formula**  
- This measure shows the total value of inventory increases during a specified period by calculating the actual cost amount and filtering only those item ledger entries that represent stock increases including purchases, positive adjustments, outputs, and assembly outputs.

**Data Sources**
- Value Entry

---
### Decreases Value
**Formula**  
- This measure shows the total value of inventory decreases during a specified period by calculating the actual cost amount and filtering only those item ledger entries that represent stock decreases including sales, negative adjustments, consumptions, and assembly consumptions.

**Data Sources**
- Value Entry

---
### Beginning Balance Value
**Formula**  
- This measure shows the total value of inventory at the beginning of a specified period by calculating the actual cost amount in the Value Entry table prior to the beginning of the specified period.

**Data Sources**
- Value Entry

---
### Ending Balance Value
**Formula**  
- This measure calculates calculates the total value of inventory at the end of a specific period.

  *Ending Balance Value = Beginning Balance Value + Net Balance Value*

**Data Sources**
- Value Entry

---
### Ending Balance Posted to G/L
**Formula**  
- This measure calculates the total value of inventory posted to the general ledger at the end of a specified period.

  *Ending Balance Posted to G/L = Beginning Balance G/L + Net Balance G/L*

**Data Sources**
- Value Entry

---
### Variance
**Formula**  
- This measure calculates the difference between the total value of inventory to the general ledger and the total value of inventory at the end of a specified period.

  *Variance = Ending Balance Posted to G/L - Ending Balance Value*

**Data Sources**
- Value Entry

---
### Invoiced Quantity
**Formula**  
- This measure calculates the total quantity of inventory that has been invoiced during a specific period by summing the invoiced quantity in the Value Entry table.

**Data Sources**
- Value Entry

---
### Increases Qty
**Formula**  
- This measure shows the total quantity of inventory increases during a specified period by calculating the invoiced quantity in the Value Entry table and filtering only those item ledger entries that represent quantity increases including purchases, positive adjustments, outputs, and assembly outputs.

**Data Sources**
- Value Entry

---
### Decreases Qty
**Formula**  
- This measure shows the total quantity of inventory decreases during a specified period by calculating the invoiced quantity in the Value Entry table and filtering only those item ledger entries that represent quantity decreases including sales, negative adjustments, consumptions, and assembly consumptions.

**Data Sources**
- Value Entry

---
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]


## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of inventory valuation data](#TODO)   
[Built-in inventory valuation reports](#TODO)   
[Inventory valuation analytics overview](#TODO)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
