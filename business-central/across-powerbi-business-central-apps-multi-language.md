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


# Multi-language Power BI apps for Business Central

In this article, you learn how to test multi-language capabilities in the Power BI apps for Business Central. 

> [!IMPORTANT]
> Power BI apps for Finance, Sales, Purchase, Inventory, Manufacturing, and Projects in Business Central is currently in PREVIEW.
> This information relates to a prerelease product that may be substantially modified before it's released. Microsoft makes no warranties, expressed or implied, with respect to the information provided here.

<!-- TODO: replace with 
[!INCLUDE [preview](includes/preview.md)] 
-->

## Languages and locales in the preview

In the preview, the following languages and locales are available: 
* en-US, 
* es-ES, 
* fr-FR, and 
* de-DE.

The following apps are currently available in multi-language
* finance


## How to try a Power BI app in a languages/locales

Initially in the preview, you can try languages/locales for a Power BI app in the Power BI service. Later, the embed experience in Business Central will also display reports in the language/locale of the Business Central user. 

To try an app in a language, simply add `language = <culture name>` to the url parameters. For example, this URL will show an app in German:
* https://<your domain>.powerbi.com/groups/a1d27337-134a-4326-99ed-9e68a1485679/reports/3173137b-a485-42e2-a3df-8f3acd7640a6/ReportSection2fa580b0181e8c981cdc?experience=power-bi&language=de-DE


## Languages and locales 

A culture name is usually a lower-case language identifier and an upper-case locale identifier separated by a hyphen. The culture name `en-US` identifies a user in the United States who speaks English. A culture name of `es-ES` identifies a user in Spain who speaks Spanish. A culture name of `fr-FR` identifies a user in France who speaks French. A culture name of `de-DE` identifies a user in Germany who speaks German.

| language parameter | Language | Locale        |
|--------------------|----------|---------------|
| en-US              | English  | United States |
| es-ES              | Spanish  | Spain         |
| fr-FR              | French   | France        |
| de-DE              | German   | Germany       |

## See also

<!-- TODO when merging to docs repo: update with relevant See also links -->