---
title: Configure the Power BI finance app for Business Central
description: Learn how to configure the finance Power BI app for your Business Central finance data.
author: kennieNP
ms.topic: get-started
ms.devlang: al
ms.search.keywords: analysis, reporting, business intelligence, KPI, installation, administration
ms.date: 05/28/2024
ms.author: kepontop
ms.service: dynamics-365-business-central
---

<!-- TODO: 
Replace
Power BI
with 
[!INCLUDE [powerbi-name](includes/powerbi-name.md)]

Replace
Power BI PRO
with 
[!INCLUDE [powerbi-pro](includes/powerbi-pro-license-name.md)]

Replace
Business Central
with 
[!INCLUDE [prod_short](includes/prod_short.md)] 


-->


# Configure the Power BI finance app for Business Central

In this article, you learn how to configure the Power BI finance app for Business Central. The app include APIs for reading finance data, Power BI semantic models and reports, and pages that embeds the Power BI finance reports in the Business Central client including navigation links from relevant role centers.

> [!IMPORTANT]
> Power BI apps for Finance, Sales, Purchase, Inventory, Manufacturing, and Projects in Business Central is currently in PREVIEW.
> This information relates to a prerelease product that may be substantially modified before it's released. Microsoft makes no warranties, expressed or implied, with respect to the information provided here.

<!-- TODO: replace with 
[!INCLUDE [preview](includes/preview.md)] 
-->

## Prerequisites

Before you can configure the Power BI finance app for Business Central, you need to install both the connector app (provides the APIs for reading data, configuration pages, and embed pages) and the Power BI app (provides the semantic model and reports)

For more information, see [Install Power BI apps for Business Central](across-powerbi-install-business-central-apps.md).

## Configure the Power BI workspace



## Configure the G/L account category mapping

G/L Account Categories in Microsoft Dynamics 365 Business Central allow you to group accounts in your chart to specific categories used for reporting. They are required set up to use the Power BI Finance app for Business Central.

### What do I need to set up?

For each posting account in the Chart of Accounts, an Account Category and Account Subcategory need to be set. Totalling accounts do not require this to be set up.

### How do I assign G/L Accounts to categories?

The Account Category and Account Subcategory can be assigned directly to the G/L Account via the G/L Account Card.

Alternatively, the G/L Account Categories summary page can be used.

### Can I create my own categories?

Yes. However, you must leave the following top-level categories as-is:
- Assets
- Liabilities
- Equity
- Income
- Cost of Goods Sold
- Expense

Subcategories can be created through the G/L Account Categories screen, in conjunction with the Indent, Outdent, Move Up and Move Down actions.

### What is the standard configuration?

This standard configuration is the default mapping of Business Central G/L account categories to the corresponding parameters in the Power BI Finance report semantic model.

### Level 1 Categories

| Parameter                                 | Business Central Category |
| ---                                       | ---                       |
| Assets (Level 1 Category)                 | Assets                    |
| Liabilities (Level 1 Category)            | Liabilities               |
| Equity (Level 1 Category)                 | Equity                    |
| Revenue (Level 1 Category)                | Income                    |
| Cost of Goods Sold (Level 1 Category)     | Cost of Goods Sold        |
| Expense (Level 1 Category)                | Expense                   |


### Level 2 Categories

| Parameter                                        	| Business Central Category     	|
|--------------------------------------------------	|-------------------------------	|
| Current Assets (Level 2 Category)                	| Current Assets                	|
| Current Liabilities (Level 2 Category)           	| Current Liabilities           	|
| Shareholder's Equity (Level 2 Category)          	| Common Stock                  	|
| Interest Expense (Level 2 Category)             	| Interest Expense                 	|
| Tax Expense (Level 2 Category)                   	| Tax Expense                   	|
| Extraordinary Expense (Level 2 Category)         	| Extraordinary Expense             |
| FX Losses Expense (Level 2 Category)             	| FX Losses Expense                 |      	
| Depreciation and Amortization (Level 2 Category) 	| Depreciation and Amortization     |
| Interest Revenue (Level 2 Category)              	| Interest Income                	|
| FX Gains Revenue (Level 2 Category)              	| FX Gains Income                   |
| Extraordinary Revenue (Level 2 Category)         	| Extraordinary Income          	|
| Fixed Assets (Level 2 Category)                  	| Fixed Assets                      |
| Payroll Liabilities (Level 2 Category)           	| Payroll Liabilities               |
| Longterm Liabilities (Level 2 Category)          	| Long Term Liabilities           	|


### Level 3 Categories

| Parameter                                 | Business Central Category |
| ---                                       | ---                       |
| Inventory (Level 3 Category)              | Inventory                 |
| Accounts Payable (Level 3 Category)       | Accounts Payable          |
| Accounts Receivable (Level 3 Category)    | Accounts Receivable       |
| Purchases (Level 3 Category)              | Purchases                 |
| Purchase Prepayments (Level 3 Category)   | Prepaid Expenses          |
| Liquid Assets (Level 3 Category)          | Cash                      |