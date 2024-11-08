---
title: Projects KPIs and measures (Power BI)
description: The Projects App KPIs provides a page to clearly identify all KPIs and Measures used in the Projects Report.
author: kennienp
ms.author: kepontop
ms.reviewer: 
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 
ms.date: 11/08/2024
ms.service: dynamics-365-business-central
---

# Power BI Projects app KPIs and measures

[!INCLUDE[applies-to-2024w2](includes/applies-to-2024w2.md)]

This page provides a list of all Key Performance Indicators (KPIs) included in the semantic model for the Power BI Projects report. 

Explore the list of KPIs below to learn more about how they can help you achieve your business goals. 

Each KPI is described, including how it is calculated and what data was used in the calculations.

---
### % Invoiced
**Formula**  
- This measure calculates the percentage of billable amount that has been invoiced to customers.

  *% Invoiced = Billable (Invoiced Price) / Billable (Total Price)*
  
**Data Sources**
- Job Ledger Entry
- Job Planning Line

---
### Quantity
**Formula**  
- This measure calculates the total quantity of a product or service used in a project by summing the quantity in the Project Ledger Entry table and converting the measure to a postive value.
  
**Data Sources**
- Job Ledger Entry

---
### Billable (Invoiced Price)
**Formula**  
- This measure shows the total invoiced price of billable project entries by calculating the total price (in local currency) in the Project Ledger Entry table and selecting only those entries with an entry type of "Sale", which indicates that the project entry is billable.
  
**Data Sources**
- Job Ledger Entry

---
### Billable (Total Price)
**Formula**  
- This measure shows the total billable amount of project planning lines by calculating the total price (in local currency) in the Project Planning Line table and selecting only those lines with a line type of "Billable" or "Both Budget and Billable", which indicates that the line is billable.
  
**Data Sources**
- Job Planning Line

---
### Actual (Total Price)
**Formula**  
- This measure calculates the total actual cost of project entries by calculating the total price (in local currency) in the Project Ledger Entry table and selecting only those entries with an entry type of "Usage". The result of this calculation is then converted to a positive value.
  
**Data Sources**
- Job Ledger Entry


---
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]


## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of projects data](#TODO)   
[Built-in projects reports](#TODO)   
[Projects analytics overview](#TODO)  
[Projects overview](#TODO)

[!INCLUDE[footer-include](includes/footer-banner.md)]
