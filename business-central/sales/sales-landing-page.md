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

| Report | Usage examples | Learn more |
| ------ | -------------- | ---------- |
| Sales Overview | The Sales Overview can be used to show high level information on sales activities. This can be used to quickly identify Sales figures relating to Quantity or Amounts and both posted and unposted documents. This can assist, supporting order processing having a view of different order documents and key metrics on Salespeople, Customers and Items. | [Sales Overview](#TODO) |
| Daily Sales | The Daily Sales report indicates the value of Sales across different days. This can highlight different daily trends and help identify the busiest days. Users can also compare days across multiple periods.| [Daily Sales](#TODO) |
| Moving Average | The moving averages report is used to show a 30 Day average across the Sales Amount over the course of the year. This can assist in understanding yearly trends across sales values. | [Moving Average](#TODO) |
| Moving Annual Total | The Moving Annual Total report highlights the annual total of the Sales Amount. This provides a cumlative view of a rolling 12-month period. The page can provide useful insights in determining trends and forecasting. | [Moving Annual Total](#TODO) |
| Period-Over-Period Growth | The Period-Over-Period Growth report is used to identify trends across the different periods. This can be reviewed at the year, quarter or month level and can identify how sales are tracking across these periods. | [Period-Over-Period Growth](#TODO) |
| Month-To-Date | The Month To Date report shows the growth of the Sales Amount each month. This resets at the end of the month but can be used to ensure sales are tracking for the month. | [Month-To-Date](#TODO) |
| Sales by Item | The Sales by Item report can be use to show how each Item is performing over a specific period. This can be used in conjunction with other reporting options. | [Sales by Item](#TODO) |
| Sales by Customer | The Sales by Customer report can be use to show how each customer is performing over a specific period. This can be used in conjunction with other reporting options. | [Sales by Customer](#TODO) |
| Sales by Salesperson | The Sales by Salesperson report can be use to show how each salesperson is performing over a specific period. This can be used in conjunction with other reporting options. | [Sales by Salesperson](#TODO) |
| Sales by Location |  The Sales by Salesperson report can be use to show how each location is performing over a specific period. This can be used in conjunction with other reporting options. | [Sales by Location](sales-by-location.md)  |
| Actual vs. Budget | The Actual vs Budget report can be used to make informed comparisons for sales reporting how sales is going compared to the budget. | [Actual vs. Budget](actual-vs-budget.md) |
