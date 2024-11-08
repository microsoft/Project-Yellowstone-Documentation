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

## Projects Table
- [% Invoiced](#invoiced)
- [% Complete](#complete)
- [Realization %](#realization)
- [Actual Profit](#actual-profit)
- [Actual Profit Margin %](#actual-profit-margin)
- [Project Count](#project-count)
- [Budget Profit Margin %](#budget-profit-margin-percent)
- [Realization Variance](#realization-variance)

## Project Ledger Entries Table
- [Quantity](#quantity)
- [Billable (Invoiced Price)](#billable-invoiced-price)
- [Actual (Total Price)](#actual-total-price)
- [Actual (Total Cost)](#actual-total-cost)


## Project Planning Lines Table
- [Billable (Total Price)](#billable-total-price)
- [Budget (Total Cost)](#budget-total-cost)
- [Budget (Total Price)](#budget-total-price)
- [Total Cost Variance to Budget](#total-cost-variance-to-budget)
- [Total Cost Variance to Budget %](#total-cost-variance-to-budget-percent)

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
### % Complete
**Formula**  
- This measure calculates the percentage of the project that has been completed based on the actual total cost and the budgeted total cost.

  *% Complete = Actual (Total Cost) / Budget (Total Cost)*
  
**Data Sources**
- Job Ledger Entry
- Job Planning Line

---
### Realization %
**Formula**  
- This measure calculates the percentage of project invoiced price that has been realized based on the actual total cost.

  *Realization % = Billable (Invoiced Price) / Actual (Total Price)*
  
**Data Sources**
- Job Ledger Entry

---
### Actual Profit
**Formula**  
- This measure represents the actual profit of a project.

  *Actual Profit = Billable (Invoiced Price) - Actual (Total Cost)*
  
**Data Sources**
- Job Ledger Entry

---
### Actual Profit Margin %
**Formula**  
- This measure represents the actual profit margin percentage of a project.

  *Actual Profit Margin % = Actual Profit / Billable (Invoiced Price)*
  
**Data Sources**
- Job Ledger Entry

---
### Actual (Total Cost)
**Formula**  
- This measure represents the actual cost of resources used in the project by calculating the total cost (in local currency) in the Project Ledger Entry table and selecting only those entries with an entry type of "Usage".
  
**Data Sources**
- Job Ledger Entry

---
### Budget (Total Cost)
**Formula**  
- This measure represents the budgeted cost of resources to be used in a project by calculating the total cost (in local currency) in the Project Planning Line table and selecting only those lines with a line type of "Budget" or "Both Budget and Billable".

**Data Sources**
- Job Ledger Entry

---
### Project Count
**Formula**  
- This measure counts the total number of projects in the Project table.

**Data Sources**
- Job

---
### Budget (Total Price)
**Formula**  
- This measure represents the budgeted price of resources to be used in a project by calculating the total price (in local currency) in the Project Planning Line table and selecting only those lines with a line type of "Budget" or "Both Budget and Billable".

**Data Sources**
- Job Planning Line

---
### Total Cost Variance to Budget
**Formula**  
- This measure calculates the variance between the actual total cost and the budgeted total cost of a project.

  *Total Cost Variance to Budget = Actual (Total Cost) - Budget (Total Cost)*

**Data Sources**
- Job Ledger Entry

---
### Total Cost Variance to Budget %
**Formula**  
- This measure calculates the variance between the actual total cost and the budgeted total cost of a project, expressed as a percentage.

  *Total Cost Variance to Budget % = Total Cost Variance to Budget / Budget (Total Cost)*

**Data Sources**
- Job Ledger Entry

---
### Budget Profit Margin %
**Formula**  
- This measure calculates the profit margin percentage for a project based on the budgeted profit and the budgeted total price of the project.

  *Budget Profit Margin % = Budget Profit / Budget (Total Price)*

**Data Sources**
- Job Ledger Entry
- Job Planning Line

---
### Realization Variance
**Formula**  
- This measure calculates the variance between the billable amount and the actual total cost of a project.

  *Realization Variance = Billable (Invoiced Price) - Actual (Total Price)*

**Data Sources**
- Job Ledger Entry
- Job Planning Line

---
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]


## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of projects data](#TODO)   
[Built-in projects reports](#TODO)   
[Projects analytics overview](#TODO)  
[Projects overview](#TODO)

[!INCLUDE[footer-include](includes/footer-banner.md)]
