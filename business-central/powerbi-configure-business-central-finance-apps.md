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

Before configuring the Power BI finance app for Business Central, you must have:

1. The Finance Connector app:
   - This app provides the APIs for data access, configuration pages, and embed pages. Make sure that the app is installed in your environment.
2. The Finance Power BI app: 
   - This app provides the semantic model and reports. Make sure that the app is installed in your Power BI workspace.

For more information, see [Install Power BI apps for Business Central](across-powerbi-install-business-central-apps.md).



## Configure date filtering for the Finance Connector

This section describes how to configure the date filtering for the Finance Connector app. The Finance Report can be configured to load data based on the **Start Date** and **End Date**. This filter helps improve performance of your Business Central environment and reduce Power BI load times by only loading the data you intend to analyze.

The **Start Date** and **End Date** can be applied to the following tables:
- G/L Entries (related to the Income Statement)
- G/L Budget Entries
- Customer Ledger Entries
- Vendor Ledger Entries


### Setup Procedure
1. Search and open the **Setup for Power BI Connector** page.
2. Expand the **Finance Report** section in this page.
3. Set **Start Date** and **End Date** under the **Income Statement & G/L Budget Entry Filters** group.

Repeat steps 2-3 for the date setup under **Customer Ledger Entry Filters** and **Vendor Ledger Entry Filters**.


The following fields are available on the **Setup for Power BI Connector** page:


|No.| Data Area                         | Field Name    | Description                                                                                               |
|---| ---                               | ---           | ---                                                                                                       |
|1  | Income Statement and G/L Budgets	| Start Date    | Specifies the starting date to apply to a range of Income Statement G/L entries and G/L Budget entries.   |
|2  | Income Statement and G/L Budgets	| End Date      | Specifies the end date to apply to a range of Income Statement G/L entries and G/L Budget entries.        |
|3  | Customer Ledger Entries	        | Start Date    | Specifies the starting date to apply to a range of Customer Ledger Entries.                               |  
|4  | Customer Ledger Entries	        | End Date      | Specifies the end date to apply to a range of Customer Ledger Entries.                                    |
|5  | Vendor Ledger Entries	            | Start Date    | Specifies the starting date to apply to a range of Vendor Ledger Entries.                                 |
|6  | Vendor Ledger Entries	            | End Date      | Specifies the end date to apply to a range of Vendor Ledger Entries.                                      |

## Configure the G/L account category mapping

In Business Central, **G/L Account Categories** allow you to group accounts in your chart for reporting purposes and these categories are essential for using the **Power BI Finance** app.

### What do I need to set up?

For each posting account in the Chart of Accounts, you must set an **Account Category** and **Account Subcategory**. You do not need to set up the totalling accounts.

### How do I assign G/L Accounts to categories?

The **Account Category** and **Account Subcategory** can be assigned on the **G/L Account Card** page. Alternatively, the **G/L Account Categories** list page can be used.

### Can I create my own categories?

Yes. However, you must leave the following top-level categories as is:
- **Assets**
- **Liabilities**
- **Equity**
- **Income**
- **Cost of Goods Sold**
- **Expense**

The subcategories can be created through **the G/L Account Categories** page, in conjunction with the **Indent**, **Outdent**, **Move Up** and **Move Down** actions.

### What is the standard configuration?

This standard configuration is the default mapping of the corresponding parameters in the Power BI Finance semantic model to the **G/L Account Categories** in Business Central.

### Level 1 Categories
Level 1 categories are the top-level categories without any indentation.

| Parameter                                 | Business Central Category |
| ---                                       | ---                       |
| Assets (Level 1 Category)                 | Assets                    |
| Liabilities (Level 1 Category)            | Liabilities               |
| Equity (Level 1 Category)                 | Equity                    |
| Revenue (Level 1 Category)                | Income                    |
| Cost of Goods Sold (Level 1 Category)     | Cost of Goods Sold        |
| Expense (Level 1 Category)                | Expense                   |


### Level 2 Categories
Level 2 categories are the second-level categories with indentation.

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
Level 3 categories are the subcategories of Level 2 with indentation.

| Parameter                                 | Business Central Category |
| ---                                       | ---                       |
| Inventory (Level 3 Category)              | Inventory                 |
| Accounts Payable (Level 3 Category)       | Accounts Payable          |
| Accounts Receivable (Level 3 Category)    | Accounts Receivable       |
| Purchases (Level 3 Category)              | Purchases                 |
| Purchase Prepayments (Level 3 Category)   | Prepaid Expenses          |
| Liquid Assets (Level 3 Category)          | Cash                      |


## Fixing problems 
### "Column ‘G/L Account No.’ in Table ‘G/L Account’ contains a duplicate value"

When refreshing data from your Business Central environment into the Finance Power BI app, a refresh error may occur due to how your **Begin-Total** and **End-Total** accounts are configured in your **Chart of Accounts**. 

If you receive this error, please review the totalling accounts.

```
Something went wrong
There was an error when processing the data in the dataset.
Please try again later or contact support. If you contact support, please provide these details.

Data source error: Column 'G/L Account No.' in Table 'G/L Account' contains a duplicate value 'X' and this is not allowed for columns on the one side of a many-to-one relationship or for columns that are used as the primary key of a table.
```

### Cause

This is due to the Finance Connector app relying on the totalling accounts for hierarchy and indentation purposes.

Your totalling for an **End-Total** account must exactly reference both the **Begin-Total** and **End-Total** accounts. This means one **Begin-Total** account can only be used in one **End-Total** account.

### Fixing the totalling on your G/L Accounts
The totalling accounts should be set up such as the following example:

1. A Begin-Total account of **1300 (Vehicles)** and the End-Total account of **1390 (Vehicles, Total)**.
2. The totalling defined on the End-Total is **1300..1390**. 
3. If your totalling account is defined as any other combination (such as 1300..1340, 1310..1390, or 1310..1340, etc.), this will cause the error.
4. One **Begin-Total** account can only be used in one **End-Total** account. If you use a **Begin-Total** account in two or more **End-Total** accounts, then the Finance Power BI app cannot match it to an **End-Total** account.
