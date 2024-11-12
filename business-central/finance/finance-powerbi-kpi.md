---
title: Finance App KPIs and measures (Power BI)
description: Get an overview of all the KPIs and measures in the semantic model for the Finance Power BI app.
author: kennienp
ms.author: kepontop
ms.reviewer:
ms.topic: conceptual
ms.search.keywords: reporting
ms.search.form: 
ms.date: 10/31/2024
ms.service: dynamics-365-business-central
---

# Power BI Finance app KPIs and measures

[!INCLUDE[applies-to-2024w2](includes/applies-to-2024w2.md)]

This page provides a list of all Key Performance Indicators (KPIs) included in the semantic model for the Power BI Finance report. 

Explore the list of KPIs below to learn more about how they can help you achieve your business goals. 

Each KPI is described, including how it is calculated and what data was used in the calculations.

---
[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]

- [Activity KPIs](#activity-kpis)
- [Balance Sheet Measures](#balance-sheet-measures)
- [Income Statement Measures](#income-statement-measures)
- [Liquidity KPIs](#liquidity-kpis)
- [Profitability KPIs](#profitability-kpis)
- [Customer Ledger Measures](#customer-ledger-measures)
- [Vendor Ledger Measures](#vendor-ledger-measures)
- [G/L Entry Meaures](#gl-entry-measures)
- [G/L Budget Entry Meaures](#gl-budget-entry-measures)

## Activity KPIs

- [% Change in Operating Profit - EBIT](#-change-in-operating-profit---ebit) 
- [% Change in Revenue](#-change-in-revenue) 
- [Asset Turnover Ratio](#asset-turnover-ratio)  
- [Average Collection Period (Days)](#average-collection-period-days)  
- [Cash Conversion Cycle - CCC](#cash-conversion-cycle---ccc)
- [Days Payable Outstanding - DPO](#days-payable-outstanding---dpo)  
- [Days Sales Of Inventory - DSI](#days-sales-of-inventory---dsi)  
- [Days Sales Outstanding - DSO](#days-sales-outstanding---dso)  
- [Degree Of Operating Leverage - DOL](#degree-of-operating-leverage---dol)  
- [Inventory Turnover](#inventory-turnover)  


### % Change in Operating Profit - EBIT
**Formula**  
( [Operating Profit - EBIT (Balance at Date)] - [Operating Profit - EBIT (Beginning Balance)] ) / [Operating Profit - EBIT (Beginning Balance)]

**Data Sources**
- G/L Entry
- G/L Account Category

### % Change in Revenue 
**Formula**  
( [Revenue (Balance at Date)] - [Revenue (Beginning Balance)] ) / [Revenue (Beginning Balance)]

**Data Sources**
- G/L Entry
- G/L Account Category

### Asset Turnover Ratio 
**Formula**  
[Revenue] / [Assets](#assets)

**Data Sources**
- G/L Entry
- G/L Account Category

### Average Collection Period (Days) 
**Formula**  
( [No. of Days] * [Accounts Receivable (Average)] ) / [Revenue]

**Data Sources**
- Date
- G/L Entry
- G/L Account Category

### Cash Conversion Cycle - CCC 
**Formula**  
[Days Sales Of Inventory - DSI] + [Days Sales Outstanding - DSO] - [Days Payable Outstanding - DPO]

**Data Sources**
- G/L Entry
- G/L Account Category

### Days Payable Outstanding - DPO 
**Formula**  
 ( [Accounts Payable](#accounts-payable) / [Cost of Goods Sold] ) * [No. of Days]

**Data Sources**
- Date
- G/L Entry
- G/L Account Category

 
### Days Sales Of Inventory - DSI 
**Formula**  
( [Inventory](#inventory) / [Cost of Goods Sold] ) * [No. of Days]

**Data Sources**
- Date
- G/L Entry
- G/L Account Category

### Days Sales Outstanding - DSO 
**Formula**  
 ( [Accounts Receivable](#accounts-receivable) / [Revenue] ) * [No. of Days]

**Data Sources**
- Date
- G/L Entry
- G/L Account Category

### Degree Of Operating Leverage - DOL 
**Formula**  
[% Change in Operating Profit - EBIT] / [% Change in Revenue]

**Data Sources**
- G/L Entry
- G/L Account Category

### Inventory Turnover
**Formula**  
[Cost of Goods Sold] / [Inventory (Average)](#inventory-average)

**Data Sources**
- G/L Entry
- G/L Account Category
## Balance Sheet Measures

- [Accounts Payable](#accounts-payable)   
- [Accounts Payable (Neg)](#accounts-payable-neg)   
- [Accounts Receivable](#accounts-receivable)   
- [Accounts Receivable (Average)](#accounts-receivable-average)   
- [Accounts Receivable (Beginning Balance)](#accounts-receivable-beginning-balance)   
- [Assets](#assets)
- [Capital Employed](#capital-employed)   
- [Current Assets](#current-assets)   
- [Current Liabilities](#current-liabilities)
- [Equity](#equity)   
- [Fixed Assets](#fixed-assets)   
- [Inventory](#inventory)   
- [Inventory (Average)](#inventory-average)   
- [Inventory (Beginning Balance)](#inventory-beginning-balance)   
- [Liabilities](#liabilities)
- [Liabilities & Equity](#liabilities--equity)   
- [Liabilities (Neg)](#liabilities-neg)   
- [Liquid Assets](#liquid-assets)   
- [Longterm Liabilities](#longterm-liabilities)   
- [Payroll Liabilities](#payroll-liabilities)   
- [Purchase Prepayments](#purchase-prepayments)   
- [Shareholders' Equity](#shareholders-equity)   
- [Working Capital](#working-capital)   

### Accounts Payable
**Formula**  
The Accounts Payable measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Accounts Payable* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Accounts Payable (Level 3 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. It then multiplies the result by -1 to display the balance as a positive value.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Accounts Payable (Neg)
**Formula**  
The Accounts Payable measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Accounts Payable* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Accounts Payable (Level 3 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories
 
### Accounts Receivable
**Formula**  
The Accounts Receivable measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Accounts Receivable* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Accounts Receivable (Level 3 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Accounts Receivable (Average) 
**Formula**  
( [Accounts Receivable (Beginning Balance)](#accounts-receivable-beginning-balance) + [Accounts Receivable](#accounts-receivable) ) / 2

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Accounts Receivable (Beginning Balance) 
**Formula**  
The Accounts Receivable (Beginning Balance) measure calculates the `[Balance at Date]` for [accounts receivable](#accounts-receivable) up to the earliest date in the selected period. The measure calculates the beginning balance by identifying the earliest date in the selected period, removing any existing date filters to consider all historical dates, and then limiting results to transactions on or before this earliest date. This approach yields the balance as of the start of the selected period.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Assets
**Formula**  
The Assets measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Assets* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Assets (Level 1 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Current Assets
**Formula**  
The Current Assets measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Current Assets* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Current Assets (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Fixed Assets
**Formula**  
The Fixed Assets measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Fixed Assets* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Fixed Assets (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Inventory
**Formula**  
The Inventory measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Inventory* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Inventory (Level 3 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Inventory (Average)
**Formula**  
( [Inventory (Beginning Balance)](#inventory-beginning-balance) + [Inventory](#inventory) ) / 2

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Inventory (Beginning Balance) 
**Formula**  
The Inventory (Beginning Balance) measure calculates the `[Balance at Date]` for [Inventory](#inventory) up to the earliest date in the selected period. The measure calculates the beginning balance by identifying the earliest date in the selected period, removing any existing date filters to consider all historical dates, and then limiting results to transactions on or before this earliest date. This approach yields the balance as of the start of the selected period.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Liquid Assets
**Formula**  
The Liquid Assets measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Cash* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Liquid Assets (Level 3 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Capital Employed
**Formula**  
[Assets](#assets) - [Current Liabilities](#current-liabilities)

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 
 
### Equity
**Formula**  
The Equity measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Equity* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Equity (Level 1 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 

### Current Liabilities
**Formula**  
The Current Liabilities measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Current Liabilities* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Current Liabilities (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. It then multiplies the result by -1 to display the balance as a positive value.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 
### Liabilities

**Formula**  
The Liabilities measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Liabilities* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Liabilities (Level 1 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. It then multiplies the result by -1 to display the balance as a positive value.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 
 
### Liabilities (Neg)
**Formula**  
The Liabilities measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Liabilities* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Liabilities (Level 1 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 

### Liabilities & Equity  
**Formula**  
[Liabilities](#liabilities) + [Equity](#equity)

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 

### Longterm Liabilities  
**Formula**  
The Longterm Liabilities measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Longterm Liabilities* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Longterm Liabilities (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. It then multiplies the result by -1 to display the balance as a positive value.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 
 
### Payroll Liabilities   
**Formula**  
The Payroll Liabilities measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Payroll Liabilities* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Payroll Liabilities (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. It then multiplies the result by -1 to display the balance as a positive value.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 
 
### Purchase Prepayments   
**Formula**  
The Purchase Prepayments measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Purchase Prepayments* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Purchase Prepayments (Level 3 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 
 
### Shareholders Equity   
**Formula**  
The Shareholders Equity measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Common Stock* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Shareholder's Equity (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 
   
### Working Capital 
**Formula**  
[Current Assets](#current-assets) + [Current Liabilities](#current-liabilities)

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories 
 
## Income Statement Measures
- [Cost of Goods Sold](#cost-of-goods-sold)
- [Depreciation and Amortization](#depreciation-and-amortization)
- [Expense](#expense) 
- [Expense (Balance at Date)](#expense-balance-at-date)  
- [Expense (Beginning Balance)](#expense-beginning-balance)  
- [Extraordinary Expense](#extraordinary-expense)   
- [Extraordinary Expense (Balance at Date)](#extraordinary-expense-balance-at-date)   
- [Extraordinary Expense (Beginning Balance)](#extraordinary-expense-beginning-balance)   
- Extraordinary Revenue   
- Extraordinary Revenue (Balance at Date)   
- Extraordinary Revenue (Beginning Balance)   
- [FX Gains Revenue](#fx-losses-expense)   
- [FX Gains Revenue (Balance at Date)](#fx-losses-expense-balance-at-date)   
- [FX Gains Revenue (Beginning Balance)](#fx-losses-expense-beginning-balance)   
- FX Losses Expense   
- FX Losses Expense (Balance at Date)   
- FX Losses Expense (Beginning Balance)   
- Interest Expense   
- Interest Expense (Balance at Date)   
- Interest Expense (Beginning Balance)   
- Interest Revenue    
- Interest Revenue (Balance at Date)   
- Interest Revenue (Beginning Balance)   
- Operating Expense - OPEX 
- Operating Expense - OPEX (Balance at Date)   
- Operating Expense - OPEX (Beginning Balance)    
- Operating Revenue   
- Operating Revenue (Balance at Date)   
- Operating Revenue (Beginning Balance)   
- Purchases   
- Revenue 
- Revenue (Balance at Date) 
- Revenue (Beginning Balance) 
- Tax Expense   
- Tax Expense (Balance at Date)   
- Tax Expense (Beginning Balance)   

### Cost of Goods Sold
**Formula**  
The Cost of Goods Sold measure calculates the `[Net Change]` for general ledger accounts categorized as *Cost of Goods Sold* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Cost of Goods Sold (Level 1 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Depreciation and Amortization
**Formula**  
The Depreciation and Amortization measure calculates the `[Net Change]` for general ledger accounts categorized as *Depreciation and Amortization* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Depreciation and Amortization Expense (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Expense
**Formula**  
The Expense measure calculates the `[Net Change]` for general ledger accounts categorized as *Expense* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Expense (Level 1 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Expense (Balance at Date)  
**Formula**  
The Expense measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Expense* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Expense (Level 1 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Expense (Beginning Balance)  
**Formula**  
The Expense (Beginning Balance) measure calculates the `[Balance at Date]` for [Expense](#expense) up to the earliest date in the selected period. The measure calculates the beginning balance by identifying the earliest date in the selected period, removing any existing date filters to consider all historical dates, and then limiting results to transactions on or before this earliest date. This approach yields the balance as of the start of the selected period.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Extraordinary Expense
**Formula**  
The Extraordinary Expense measure calculates the `[Net Change]` for general ledger accounts categorized as *Extraordinary Expense* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Extraordinary Expense (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Extraordinary Expense (Balance at Date)
**Formula**  
The Extraordinary Expense measure calculates the `[Balance at Date]` for general ledger accounts categorized as *Extraordinary Expense* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **Extraordinary Expense (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### Extraordinary Expense (Beginning Balance)  
**Formula**  
The Extraordinary Expense (Beginning Balance) measure calculates the `[Balance at Date]` for [Extraordinary Expense](#extraordinary-expense) up to the earliest date in the selected period. The measure calculates the beginning balance by identifying the earliest date in the selected period, removing any existing date filters to consider all historical dates, and then limiting results to transactions on or before this earliest date. This approach yields the balance as of the start of the selected period.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories





### FX Losses Expense
**Formula**  
The FX Losses Expense measure calculates the `[Net Change]` for general ledger accounts categorized as *FX Losses Expense* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **FX Losses (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### FX Losses Expense (Balance at Date)
**Formula**  
The FX Losses Expense measure calculates the `[Balance at Date]` for general ledger accounts categorized as *FX Losses Expense* on the [G/L Account Category](https://businesscentral.dynamics.com?page=790) page and where this category is mapped to the **FX Losses Expense (Level 2 Category)** on the [Power BI Account Categories](https://businesscentral.dynamics.com?page=36961) page. 

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories

### FX Losses Expense (Beginning Balance)  
**Formula**  
The FX Losses Expense (Beginning Balance) measure calculates the `[Balance at Date]` for [FX Losses Expense](#fx-losses-expense) up to the earliest date in the selected period. The measure calculates the beginning balance by identifying the earliest date in the selected period, removing any existing date filters to consider all historical dates, and then limiting results to transactions on or before this earliest date. This approach yields the balance as of the start of the selected period.

**Data Sources**
- G/L Entry
- G/L Account Category
- Account Categories













## See also

[Track your business KPIs with Power BI metrics](#TODO)   
[Ad-hoc analysis of projects data](#TODO)   
[Built-in projects reports](#TODO)   
[Projects analytics overview](#TODO)  
[Projects overview](#TODO)

[!INCLUDE[footer-include](includes/footer-banner.md)]