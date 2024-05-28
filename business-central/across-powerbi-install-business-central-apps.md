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

# Install [!INCLUDE [prod_short](includes/powerbi-name.md)] apps for [!INCLUDE [prod_short](includes/prod_short.md)]

In this article, you learn how to install the [!INCLUDE [prod_short](includes/powerbi-name.md)] apps for [!INCLUDE [prod_short](includes/prod_short.md)]. The apps are specific to each functional area of [!INCLUDE [prod_short](includes/prod_short.md)] and include APIs for reading data, [!INCLUDE [prod_short](includes/powerbi-name.md)] semantic models and reports, and pages that embeds the [!INCLUDE [prod_short](includes/powerbi-name.md)] reports in the [!INCLUDE [prod_short](includes/prod_short.md)] client including navigation links from relevant role centers.

[!INCLUDE [prod_short](includes/preview.md)]

## Prerequisites

To install [!INCLUDE [prod_short](includes/powerbi-name.md)] apps for [!INCLUDE [prod_short](includes/prod_short.md)], you need to have
- an environment in BC online (it is already set up to integrate with [!INCLUDE [prod_short](includes/powerbi-name.md)].)
- a [!INCLUDE [prod_short](includes/powerbi-pro-license-name.md)] license for the user who is installing the [!INCLUDE [prod_short](includes/powerbi-name.md)] template app, the user who will be used for refreshing the data, and for each user who will access the reports. For more information, see [Get started with Power BI reports in Business Central](https://learn.microsoft.com/dynamics365/business-central/across-working-with-powerbi#get-started).

## Installing a Power BI app 

[!INCLUDE [prod_short](includes/powerbi-name.md)] apps are available for the following functional areas in [!INCLUDE [prod_short](includes/prod_short.md)]:
- Finance
- Sales
- Purchasing
- Inventory
- Warehouse
- Projects

Each app consists of two parts:
- A connector (AL) app that contains APIs, setup pages, and embed pages
- A [!INCLUDE [prod_short](includes/powerbi-name.md)] template app that contains a [!INCLUDE [prod_short](includes/powerbi-name.md)] semantic model and [!INCLUDE [prod_short](includes/powerbi-name.md)] reports.

Both apps needs to be installed for the [!INCLUDE [prod_short](includes/powerbi-name.md)] reports to work on a functional area.

### Installing the connector (AL) app

Preview only: You install the [!INCLUDE [prod_short](includes/powerbi-name.md)] connector (AL) app by using the install file (.app) supplied in the preview program.

### Installing the [!INCLUDE [prod_short](includes/powerbi-name.md)] template app

Preview only: You install the [!INCLUDE [prod_short](includes/powerbi-name.md)] template app by using the install link supplied in the preview program.

When installing the [!INCLUDE [prod_short](includes/powerbi-name.md)] template app in your [!INCLUDE [prod_short](includes/powerbi-name.md)] subscription, you need to choose a workspace for the [!INCLUDE [prod_short](includes/powerbi-name.md)] semantic model and reports. It is recommended to use one workspace for each app as this makes it easier to setup functional boundaries with access controls for which users or user groups are able to access the reports. 

> [!IMPORTANT]
> To install a Power BI template app, you need a [!INCLUDE [prod_short](includes/powerbi-pro-license-name.md)] license.



## Get the latest data

Each [!INCLUDE [prod_short](includes/powerbi-name.md)] app is based on a semantic model (also known as a dataset) that gets data from [!INCLUDE[prod_short](includes/prod_short.md)] APIs. You want to make sure that the data in your [!INCLUDE [prod_short](includes/powerbi-name.md)] reports is up to date with the data in [!INCLUDE[prod_short](includes/prod_short.md)]. This concept is referred to as *refreshing*. Depending on how your organization has set up [!INCLUDE [prod_short](includes/powerbi-name.md)], refreshing might not happen automatically. There are two ways to refresh data: manually or by scheduling a refresh. Manual refreshing is done on-demand, as needed. Scheduled refreshing lets you refresh automatically at defined time intervals.

For more information, see [Refresh Power BI semantic models](https://learn.microsoft.com/en-gb/dynamics365/business-central/across-working-with-powerbi#work-with-power-bi-reports).


## See also

<!-- TODO when merging to docs repo: update with see also links -->