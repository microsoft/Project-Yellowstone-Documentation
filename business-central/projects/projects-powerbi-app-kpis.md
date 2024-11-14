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
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]

## Project Measures
- [% Invoiced](#-invoiced)
- [% Complete](#-complete)
- Duration (Days)
- [Project Count](#project-count)
- [Realization %](#realization-)
- [Realization Variance](#realization-variance)
- Task Count

### % Invoiced

**Formula**  
*% Invoiced = [Billable (Invoiced Price)](#billable-invoiced-price) / [Billable (Total Price)](#billable-total-price)*
  
**Data Sources**
- Job Ledger Entry
- Job Planning Line

### % Complete

**Formula**  
*% Complete = [Actual (Total Cost)](#actual-total-cost) / [Budget (Total Cost)](#budget-total-cost)*
  
**Data Sources**
- Job Ledger Entry
- Job Planning Line

### Project Count
**Formula**  
The Project Count measure counts the total number of projects in the Project table.

**Data Sources**
- Job

### Realization %

**Formula**  
*Realization % = [Billable (Invoiced Price)](#billable-invoiced-price) / [Actual (Total Price)](#actual-total-price)*
  
**Data Sources**
- Job Ledger Entry

### Realization Variance

**Formula**  
*Realization Variance = [Billable (Invoiced Price)](#billable-invoiced-price) - [Actual (Total Price)](#actual-total-price)*

**Data Sources**
- Job Ledger Entry
- Job Planning Line

## Profit
- [Actual Profit](#actual-profit)
- [Actual Profit Margin %](#actual-profit-margin-)
- Budget Profit
- [Budget Profit Margin %](#budget-profit-margin-)

### Actual Profit

**Formula**  
*Actual Profit = [Billable (Invoiced Price)](#billable-invoiced-price) - [Actual (Total Cost)](#actual-total-cost)*
  
**Data Sources**
- Job Ledger Entry

### Actual Profit Margin %

**Formula**  
*Actual Profit Margin % = [Actual Profit Margin %](#actual-profit-margin-) / [Billable (Invoiced Price)](#billable-invoiced-price)*
  
**Data Sources**
- Job Ledger Entry

### Budget Profit Margin %

**Formula**  
*Budget Profit Margin % = Budget Profit / [Budget (Total Price)](#budget-total-price)*

**Data Sources**
- Job Ledger Entry
- Job Planning Line

## Project Ledger Measures
- [Actual (Total Price)](#actual-total-price)
- [Billable (Invoiced Price)](#billable-invoiced-price)
- Invoiced (Total Cost)
- Invoiced (Total Price)
- [Quantity](#quantity)
- Total Price

### Actual (Total Price)

**Formula**  
The Actual (Total Price) measure calculates the total actual cost of project entries by calculating the total price (in local currency) in the Project Ledger Entry table and selecting only those entries with an entry type of "Usage". The result of this calculation is then converted to a positive value.
  
**Data Sources**
- Job Ledger Entry


### Billable (Invoiced Price)

**Formula**  
The Billable (Invoiced Price) measure shows the total invoiced price of billable project entries by calculating the total price (in local currency) in the Project Ledger Entry table and selecting only those entries with an entry type of "Sale", which indicates that the project entry is billable.
  
**Data Sources**
- Job Ledger Entry

### Quantity

**Formula**  
The Quantity measure calculates the total quantity of a product or service used in a project by summing the quantity in the Project Ledger Entry table and converting the measure to a postive value.
  
**Data Sources**
- Job Ledger Entry

## Usage
- [Actual (Total Cost)](#actual-total-cost)
- Gen. Journal Usage (Total Cost)
- Labour Usage (Total Cost)
- Material Usage (Total Cost)


### Actual (Total Cost)

**Formula**  
The Actual (Total Cost) measure represents the actual cost of resources used in the project by calculating the total cost (in local currency) in the Project Ledger Entry table and selecting only those entries with an entry type of "Usage".
  
**Data Sources**
- Job Ledger Entry

## Planning Line Measures
- Billable (Total Cost)
- [Billable (Total Price)](#billable-total-price)
- [Budget (Total Cost)](#budget-total-cost)
- [Budget (Total Price)](#budget-total-price)
- Planning Line Quantity
- Planning Line Total Cost (LCY)
- Planning Line Total Price (LCY)
- [Total Cost Variance to Budget](#total-cost-variance-to-budget)
- [Total Cost Variance to Budget %](#total-cost-variance-to-budget-)

### Billable (Total Price)

**Formula**  
The Billable (Total Price) measure shows the total billable amount of project planning lines by calculating the total price (in local currency) in the Project Planning Line table and selecting only those lines with a line type of "Billable" or "Both Budget and Billable", which indicates that the line is billable.
  
**Data Sources**
- Job Planning Line

### Budget (Total Cost)

**Formula**  
The Budget (Total Cost) measure represents the budgeted cost of resources to be used in a project by calculating the total cost (in local currency) in the Project Planning Line table and selecting only those lines with a line type of "Budget" or "Both Budget and Billable".

**Data Sources**
- Job Ledger Entry

### Budget (Total Price)

**Formula**  
The Budget (Total Price) measure represents the budgeted price of resources to be used in a project by calculating the total price (in local currency) in the Project Planning Line table and selecting only those lines with a line type of "Budget" or "Both Budget and Billable".

**Data Sources**
- Job Planning Line

### Total Cost Variance to Budget

**Formula**  
*Total Cost Variance to Budget = [Actual (Total Cost)](#actual-total-cost) - [Budget (Total Cost)](#budget-total-cost)*

**Data Sources**
- Job Ledger Entry

### Total Cost Variance to Budget %

**Formula**  
*Total Cost Variance to Budget % = [Total Cost Variance to Budget %](#total-cost-variance-to-budget-) / [Budget (Total Cost)](#budget-total-cost)*

**Data Sources**
- Job Ledger Entry

## Purchase Measures
- Amount on PO
- Amount Rcvd. Not Invoiced
- Outstanding Amt. on PO
- Purchase Order Count
- Quantity on PO

## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of projects data](#TODO)   
[Built-in projects reports](#TODO)   
[Projects analytics overview](#TODO)  
[Projects overview](#TODO)

[!INCLUDE[footer-include](includes/footer-banner.md)]
