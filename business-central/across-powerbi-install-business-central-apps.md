---
title: Installing Power BI apps for Business Central
description: Learn how to install Power BI apps for your Business Central data.
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


# Install Power BI apps for Business Central

In this article, you learn how to install the Power BI apps for Business Central. The apps are specific to each functional area of Business Central and include APIs for reading data, Power BI semantic models and reports, and pages that embeds the Power BI reports in the Business Central client including navigation links from relevant role centers.

> [!IMPORTANT]
> Power BI apps for Finance, Sales, Purchase, Inventory, Manufacturing, and Projects in [!INCLUDE [prod_short](includes/prod_short.md)] is currently in PREVIEW.
> This information relates to a prerelease product that may be substantially modified before it's released. Microsoft makes no warranties, expressed or implied, with respect to the information provided here.

<!-- TODO: replace with 
[!INCLUDE [preview](includes/preview.md)] 
-->

## Prerequisites

To install Power BI apps for Business Central, you need to have
- an environment in BC online (it is already set up to integrate with Power BI.)
- a Power BI PRO license for the user who is installing the Power BI template app, the user who will be used for refreshing the data, and for each user who will access the reports. For more information, see [Get started with Power BI reports in Business Central](https://learn.microsoft.com/dynamics365/business-central/across-working-with-powerbi#get-started).

## Installing a Power BI app 

Power BI apps are available for the following functional areas in Business Central:
- Finance
- Sales
- Purchasing
- Inventory
- Warehouse
- Projects

Each app consists of two parts:
- A connector (AL) app that contains APIs, setup pages, and embed pages
- A Power BI template app that contains a Power BI semantic model and Power BI reports.

Both apps needs to be installed for the Power BI reports to work on a functional area.

### Installing the connector (AL) app

Preview only: You install the Power BI connector (AL) app by using the install file (.app) supplied in the preview program.

### Installing the Power BI template app

Preview only: You install the Power BI template app by using the install link supplied in the preview program.

When installing the Power BI template app in your Power BI subscription, you need to choose a workspace for the Power BI semantic model and reports. It is recommended to use one workspace for each app as this makes it easier to setup functional boundaries with access controls for which users or user groups are able to access the reports. 

> [!IMPORTANT]
> To install a Power BI template app, you need a Power BI PRO license.



## Get the latest data

Each Power BI app is based on a semantic model (also known as a dataset) that gets data from Business Central APIs. You want to make sure that the data in your Power BI reports is up to date with the data in Business Central. This concept is referred to as *refreshing*. Depending on how your organization has set up Power BI, refreshing might not happen automatically. There are two ways to refresh data: manually or by scheduling a refresh. Manual refreshing is done on-demand, as needed. Scheduled refreshing lets you refresh automatically at defined time intervals.

For more information, see [Refresh Power BI semantic models](https://learn.microsoft.com/en-gb/dynamics365/business-central/across-working-with-powerbi#work-with-power-bi-reports).


## See also

<!-- TODO when merging to docs repo: update with relevant See also links -->