# Power BI Sales App

## Overview

The Power BI Sales Report provides comprehensive sales analytics to stakeholders at all levels of the organization. Executives and the leadership team can use the [Sales Overview](sales-overview.md) report,  [Period-Over-Period Growth](period-over-period-growth.md), and [Month-To-Date](month-to-date.md) reports to identify trends in sales performance.

Managers and team leaders can track individual sales team performance using the  [Sales by Salesperson](sales-by-salesperson.md) report. They can also monitor overall team progress toward meeting sales goals by comparing actual results against targets in the [Actual vs. Budget](actual-vs-budget.md)  report.

Sales teams and other operational staff can use aggregated reports, like the [Sales by Item](sales-by-item.md) and [Sales by Customer](sales-by-customer.md) reports, to understand which items sells best and which customers are generating the most revenue. By drilling down from these aggregated views, users can seamlessly dive deep into transaction-level data for even more detailed analysis.

## Use Cases

**Target Audience**

- Executives
- Directors
- Other high-level decision makers

**Example Scenario:**
As a user, imagine you are the CEO of a company, you are preparing for an upcoming board meeting. You need to present an analysis of your company's sales performance for the current fiscal year. To better understand the company's current position, you can use the Power BI Sales report.

You first begin by reviewing the [Period-Over-Period Growth](period-over-period-growth.md) report which provides a quick comparitive view of the current year versus the previous year. You see that sales are up by 35%, outlined by the [Period-over-Period Growth %](#TODO) metric. 

![Sales Period-Over-Period screenshot](/business-central/media/sales/sales-period-over-period-fiscal-year.png "Sales Period-Over-Period - Screenshot")

Next, you review the [Sales by Customer](sales-by-customer.md) report, to see which group of customers contributed most to sales. by analyzing the Sales by Customer matrix, you can see that domestic customers outperformed foreign customers by contributing 56.59% to the total annual sales. 
![Sales-by-customer-matrix screenshot](/business-central/media/sales/sales-by-customer-matrix.png "Sales-by-customer-matrix - Screenshot")

Finally, you review the [Moving Averages](moving-average.md) report, which visualizes [Sales Amount](#TODO) and [Sales Amount Average 30D](#TODO). The 30 day average smoothes out the sales trend for the year and provides more good news for the company. This report reveals that on average, sales were stable through the first half of the year and then increased through the second half of the year. 

![30-Day-Moving-Average screenshot](/business-central/media/sales/30-Day-Moving-Average.png "30-Day-Moving-Average - Screenshot")

With the insights gained from this report, you can confidently present your organization's sales performance to the board, armed with data-driven analysis and a deeper understanding of your company's current position.

---
**Target Audience**

- Sales Manager
- Sales Team Leader

**Example Scenario:** 
As a Sales Manager, you are tasked with driving sales over the next two quarters. You turn to the Power BI Sales Report to understand the sales team's current standing. 

You begin by reviewing the [Sales by Salesperson](sales-by-salesperson.md) report to evaluate individual team performance. You quickly identify Jim Olive as the top performer, generating 83% of the total sales for the year. Using the report, you also see that Helena Ray has been the most profitable salesperson on the team but only by a small margin. 

![Sales-by-salesperson-matrix screenshot](/business-central/media/sales/sales-by-salesperson-matrix.png "Sales-by-salesperson-matrix - Screenshot")

You know that without clear targets Lina and Helena won't reach their maximum potential. By establishing a new sales budget with revised targets for each salesperson, you can provide your team with the tools they need to progress. Using the [Actual vs. Budget](actual-vs-budget.md) report, you monitor progress to ensure the team is on track to meet their new goals.

Using the [Daily Sales](daily-sales.md) report, you can monitor the team's progress over the next two quarters. Using the heat map to guage which day of the week the team performs best and when the company should roll out marketing incentives to help drive customer engagement.

![sales-daily-sales-heat-map screenshot](/business-central/media/sales/sales-daily-sales-heat-map.png "sales-daily-sales-heat-map - Screenshot")
---

**Target Audience**

- Sales Staff
- Sales People

**Example Scenario:** 
After receiving new sales targets from the Sales Manager, the sales team is eager to improve their performance and meet these revised goals. To strategize effectively, as a salesperson, you turn to the Power BI Sales Report for insights into the company's sales patterns. 

You begin by analyzing the [Sales by Item](sales-by-item.md) and [Sales by Customer](sales-by-customer.md) reports to identify high-potential products and key customers. These aggregated reports provide a clear view of where opportunities lie, allowing you to focus your efforts on customers and items most likely to generate growth and help your team achieve the targets. 

![sales-by-customer-matrix screenshot](/business-central/media/sales/sales-by-customer-matrix-2.png "sales-by-customer-matrix - Screenshot")

The [Sales by Item](sales-by-item.md) report highlights product performance by clearly identifying which items generate the most revenue and conversely which items have experienced a decline in sales. Targeting key products will allow you and your team to prioritize your efforts on highly profitable items and those with growing demand. 

![sales-by-item-matrix screenshot](/business-central/media/sales/sales-by-item-matrix.png "sales-by-item-matrix - Screenshot")

---

## Reports
The following sections provide an overview of all the available Power BI reports for sales:

| To... | Open in Business Central (CTRL+select) | Learn more |
| ------ | -------------- | ---------- | 
| Analyze high level information on sales activities. Identify sales figures relating to quantity or amounts from both posted and unposted documents.| [Sales Overview](#TODO) | [About Sales Overview](sales-overview.md) |
| Analyze sales by week day over different periods. The heatmaps highlights which days have the most sales helping you identify patterns in your sales.|[Daily Sales](#TODO)| [About Daily Sales](daily-sales.md) |
| Analyze sales trends by smoothing out spikes and drops in Sales using the 30 Day Moving Averages report. | [Moving Average](#TODO) | [About Moving Average](moving-average.md) |
| Analyze the aggregated sales over a rolling 12-month period. Use this as an alternative to a Year-to-Date report. |[Moving Annual Total](#TODO) | [About Moving Annual Total](moving-annual-total.md) |
| Compares sales in one period with the same period in a prior year, quarter, or month. |[Period-Over-Period Growth](#TODO) | [About Period-Over-Period Growth](period-over-period-growth.md) |
| Analyze accumulating sales for a desired period. | [Month-To-Date](#TODO) | [About Month-To-Date](month-to-date.md)|
| Analyze sales by item and view key metrics like Sales Amount, Sales Quantity, Cost Amount, Gross Profit, Gross Profit Margin and Sales Amount as a percent of total sales. | [Sales by Item](#TODO) | [About Sales by Item](sales-by-item.md) |
| Analyze sales by customer and view key metrics like Sales Amount, Sales Quantity, Cost Amount, Gross Profit, Gross Profit Margin and Sales Amount as a percent of total sales.  | [Sales by Customer](#TODO)  | [About Sales by Customer](sales-by-customer.md) |
| Analyze sales by salesperson and view key metrics like Sales Amount, Sales Quantity, Cost Amount, Gross Profit, Gross Profit Margin and Sales Amount as a percent of total sales.  | [Sales by Salesperson](#TODO) | [About Sales by Salesperson](sales-by-salesperson.md) |
| Analyze sales by location and view key metrics like Sales Amount, Sales Quantity, Cost Amount, Gross Profit, Gross Profit Margin and Sales Amount as a percent of total sales.  | [Sales by Location](#TODO)  | [About Sales by Location](sales-by-location.md)  |
| Analyze item sales budgets against actual sales. View target variances for both sales amounts and sales quantity. | [Actual vs. Budget](#TODO) | [About Actual vs. Budget](actual-vs-budget.md) |
