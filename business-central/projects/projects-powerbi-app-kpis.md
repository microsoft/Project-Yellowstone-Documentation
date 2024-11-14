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
- [Duration (Days)](#duration-days)
- [Project Count](#project-count)
- [Realization %](#realization-)
- [Realization Variance](#realization-variance)
- [Tasks Count](#tasks-count)

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

### Duration (Days)

**Formula**  
The Duration (Days) measure calculates the number of days between the earliest starting date and latest ending date for a given project in the Project table.
  
**Data Sources**
- Job

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

### Tasks Count

**Formula**  
The Tasks Count measure counts the number of rows in the Tasks table that where the Project Task Type has a value of "Posting".

**Data Sources**
- Job Task

## Profit
- [Actual Profit](#actual-profit)
- [Actual Profit Margin %](#actual-profit-margin-)
- [Budget Profit](#budget-profit)
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

### Budget Profit
**Formula**  
*Budget Profit = - [Budget (Total Price)](#budget-total-price) - [Budget (Total Cost)](#budget-total-cost)*

**Data Sources**
- Job Ledger Entry
- Job Planning Line

### Budget Profit Margin %

**Formula**  
*Budget Profit Margin % = [Budget Profit](#budget-profit) / [Budget (Total Price)](#budget-total-price)*

**Data Sources**
- Job Ledger Entry
- Job Planning Line

## Project Ledger Measures
- [Actual (Total Price)](#actual-total-price)
- [Billable (Invoiced Price)](#billable-invoiced-price)
- [Invoiced (Total Cost)](#invoiced-total-cost)
- [Invoiced (Total Price)](#invoiced-total-price)
- [Quantity](#quantity)
- [Total Price](#total-price)

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

### Invoiced (Total Cost)

**Formula**  
The Invoiced (Total Cost) measure calculates the total cost of all project ledger entries where the entry type is "Sale" in the Project Ledger Entry table.
  
**Data Sources**
- Job Ledger Entry

### Invoiced (Total Price)

**Formula**  
The Invoiced (Total Price) measure calculates the total price of all project ledger entries where the entry type is "Sale" in the Project Ledger Entry table.
  
**Data Sources**
- Job Ledger Entry

### Quantity

**Formula**  
The Quantity measure calculates the total quantity of a product or service used in a project by summing the quantity in the Project Ledger Entry table and converting the measure to a postive value.
  
**Data Sources**
- Job Ledger Entry

### Total Price

**Formula**  
The Total Price measure calculates the total price of all project ledger entries in the Project Ledger Entry table. It uses the SUMX function to iterate over each row in the table and multiply the quantity and unit price (in local currency) columns for each row. The results of each multiplication are then summed up to produce the total price.

**Data Sources**
- Job Ledger Entry

## Usage
- [Actual (Total Cost)](#actual-total-cost)
- [Gen. Journal Usage (Total Cost)](#gen-journal-usage-total-cost)
- [Labour Usage (Total Cost)](#labour-usage-total-cost)
- [Material Usage (Total Cost)](#material-usage-total-cost)

### Actual (Total Cost)

**Formula**  
The Actual (Total Cost) measure calculates the total cost (in local currency) of all project ledger entries where the type is "Usage" in the Project Ledger Entry table.
  
**Data Sources**
- Job Ledger Entry

### Gen. Journal Usage (Total Cost)

**Formula**  
The Gen. Journal Usage (Total Cost) measure calculates the total cost of all project ledger entries where the type is "G/L Account" in the Project Ledger Entry table.
  
**Data Sources**
- Job Ledger Entry

### Labour Usage (Total Cost)

**Formula**  
The Labour Usage (Total Cost) measure calculates the total cost of all project ledger entries where the type is "Resource" in the Project Ledger Entry table.
  
**Data Sources**
- Job Ledger Entry

### Material Usage (Total Cost)

**Formula**  
The Material Usage (Total Cost) measure calculates the total cost of all project ledger entries where the type is "Item" in the Project Ledger Entry table.
  
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
