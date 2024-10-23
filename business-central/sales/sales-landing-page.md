# Power BI Sales App

## Overview

The Power BI Sales Report provides comprehensive sales analytics to stakeholders at all levels of the organization. Executives and the leadership team can use the [Sales Overview](#TODO) report,  [Period-Over-Period Growth](#TODO), and [Month-To-Date](#TODO) reports to identify trends in sales performance.

Managers and team leaders can track individual sales team performance using the  [Sales by Salesperson](#TODO) report. They can also monitor overall team progress toward meeting sales goals by comparing actual results against targets in the [Actual vs. Budget](actual-vs-budget.md)  report.

Sales teams and other operational staff can use aggregated reports, like the [Sales by Item](#TODO) and [Sales by Customer](#TODO) reports, to understand which items sells best and which customers are generating the most revenue. By drilling down from these aggregated views, users can seamlessly dive deep into transaction-level data for even more detailed analysis.

## Use Cases

**Target Audience**

- Executives
- Directors
- Other high-level decision makers

**Example Scenario:** The CEO is preparing for an upcoming board meeting where they need to present an analysis of the organization's sales performance for the current fiscal year. To better understand the company's current position the CEO reaches for the Power BI Sales report. 

They first begin by reviweing the [Period-Over-Period Growth](#TODO) report which provides a quick comparitive view of the current year versus the previous year. They can quickly see that sales are up by 35%, outlined by the [Period-over-Period Growth %](#TODO) metric. 

![Sales Period-Over-Period screenshot](/business-central/media/sales/sales-period-over-period-fiscal-year.png "Sales Period-Over-Period - Screenshot")

Next, they review the [Sales by Customer](#TODO) report, to see which group of customers contributed most to sales. Reviewing the Sales by Customer matrix they can see that domestic customers outperformed foreign customers by contributing 56.59% to the total annual sales. 
![Sales-by-customer-matrix screenshot](/business-central/media/sales/sales-by-customer-matrix.png "Sales-by-customer-matrix - Screenshot")

Finally, the CEO reviews the [Moving Averages](#TODO) report, which visualizes [Sales Amount](#TODO) and [Sales Amount Average 30D](#TODO). The 30 day average smoothes out the sales trend for the year and provides more good news for the CEO. They can clearly see that on average, sales were stable through the first half of the year and then increased through the second half of the year. 
![30-Day-Moving-Average screenshot](/business-central/media/sales/30-Day-Moving-Average.png "30-Day-Moving-Average - Screenshot")

---
**Target Audience**

- Sales Manager
- Sales Team Leader

**Example Scenario:** 
The Sales Manager is tasked with driving sales over the next two quarters. The manager turns to the Powre BI Sales Report to understand the sales team's current standing. 

They begin by revieweing the [Sales by Salesperson](#TODO) report to evaluate individual team performance. They quickly identify Jim Olive as the top performer, generating 83% of the total sales for the year. They can also see that Helena Ray has been the most profitable salesperson on the team but only by a small margin. 

![Sales-by-salesperson-matrix screenshot](/business-central/media/sales/sales-by-salesperson-matrix.png "Sales-by-salesperson-matrix - Screenshot")

The sales manager knows that without clear targets Lina and Helena won't reach their maximum potential. By establishing a new sales budget with revised targets for each salesperson, the sales manager can provide his team with the tools they need to progress. Using the [Actual vs. Budget](actual-vs-budget.md) report, the Sales Manager monitors progress to ensure the team is on track to meet their new goals.

Using the [Daily Sales](#TODO) report the sales manager can monitor the team's progress over the next two quarters. Using the heat map to guage which day of the week the team performs best and when they should roll out marketing incentives to help drive customer engagement.

![sales-daily-sales-heat-map screenshot](/business-central/media/sales/sales-daily-sales-heat-map.png "sales-daily-sales-heat-map - Screenshot")
---

**Target Audience**

- Sales Staff
- Sales People

**Example Scenario:** After receiving new sales targets from the Sales Manager, the sales team is eager to improve their performance and meet these revised goals. To strategize effectively, they turn to the Power BI Sales Report for insights into their sales patterns. 

The team begins by analyzing the [Sales by Item](#TODO) and [Sales by Customer](#TODO) reports to identify high-potential products and key customers. These aggregated reports provide a clear view of where opportunities lie, allowing the sales team to focus their efforts on customers and items most likely to generate growth and help them achieve their targets. 

![sales-by-customer-matrix screenshot](/business-central/media/sales/sales-by-customer-matrix-2.png "sales-by-customer-matrix - Screenshot")

The [Sales by Item](#TODO) report highlights product performance by clearly identifying which items generate the most revenue and conversely which items have experienced a decline in sales. Targeting key products will allow the sales team to prioritize their efforts on highly profitable items and those with growing demand. 

![sales-by-item-matrix screenshot](/business-central/media/sales/sales-by-item-matrix.png "sales-by-item-matrix - Screenshot")

---

## Reports
The following sections provide an overview of all the available Power BI reports for sales:

| To... | Open in Business Central (CTRL+select) | Learn more |
| ------ | -------------- | ---------- | 
| Analyze high level information on sales activities. Identify sales figures relating to quantity or amounts from both posted and unposted documents.| [Sales Overview](#TODO) | [About Sales Overview](#TODO) |
| Analyze sales by week day over different periods. The heatmaps highlights which days have the most sales helping you identify patterns in your sales.|[Daily Sales](#TODO)| [About Daily Sales](#TODO) |
| Analyze sales trends by smoothing out spikes and drops in Sales using the 30 Day Moving Averages report. | [Moving Average](#TODO) | [About Moving Average](#TODO) |
| Analyze the aggregated sales over a rolling 12-month period. Use this as an alternative to a Year-to-Date report. |[Moving Annual Total](#TODO) | [About Moving Annual Total](#TODO) |
| Compares sales in one period with the same period in a prior year, quarter, or month. |[Period-Over-Period Growth](#TODO) | [About Period-Over-Period Growth](#TODO) |
| Analyze accumulating sales for a desired period. | [Month-To-Date](#TODO) | [About Month-To-Date](#TODO)|
| Analyze sales by item and view key metrics like Sales Amount, Sales Quantity, Cost Amount, Gross Profit, Gross Profit Margin and Sales Amount as a percent of total sales. | [Sales by Item](#TODO) | [About Sales by Item](#TODO) |
| Analyze sales by customer and view key metrics like Sales Amount, Sales Quantity, Cost Amount, Gross Profit, Gross Profit Margin and Sales Amount as a percent of total sales.  | [Sales by Customer](#TODO)  | [About Sales by Customer](#TODO) |
| Analyze sales by salesperson and view key metrics like Sales Amount, Sales Quantity, Cost Amount, Gross Profit, Gross Profit Margin and Sales Amount as a percent of total sales.  | [Sales by Salesperson](#TODO) | [About Sales by Salesperson](#TODO) |
| Analyze sales by location and view key metrics like Sales Amount, Sales Quantity, Cost Amount, Gross Profit, Gross Profit Margin and Sales Amount as a percent of total sales.  | [Sales by Location](sales-by-location.md)  | [About Sales by Location](sales-by-location.md)  |
| Analyze item sales budgets against actual sales. View target variances for both sales amounts and sales quantity. | [Actual vs. Budget](actual-vs-budget.md) | [About Actual vs. Budget](actual-vs-budget.md) |
