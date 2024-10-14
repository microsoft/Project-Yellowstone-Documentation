# Sales by Item (Power BI Report)

The _Sales by Item_ report gives a clear picture of your organization's Item sales. It showcases key metrics against each Item or Item Category such as Sales Amount and Quantities along with the Cost Amounts. This can be broken down further by the specific customers they are purchasing these items. 

This report is targetted towards leadership and management teams to track Item Sales. It can be used by Sales people to better identify key items.

![Sales by Item screenshot](/business-central/media/sales/sales-by-item.png "Sales by Item - Screenshot")

## What the report shows

The *Sales by Item* reports shows a clear view of total sales generated at the Item level. This can be viewable through the bar chart or the matrix view to identify amounts at different levels. The report also incorporates a drill-through ability to further breakdown specific information.


## Use Cases

**For the leadership team**

For the leadership team, *Sales by Item* report provides insights inot the top Items generating revenue for the company.
**Target Audience**

- CEO

**Example Scenario:** A CEO wants to be able to see a list of the top-selling items by revenue generated. This compared with how much each item has contributed to the company's overall revenue. This information can then be used to make strategic decisions about which products to focus on and how to allocate resources.

---

**For the management team**

For the management team, the *Sales by Item* report can be used to idenfity key performance indicators of the different items.

**Target Audience**

- Sales Manager

**Example Scenario:** A Sales Manager can identify which items aren't performing and implement sales promotions for these items. They can also use this information to adjust inventory levels of different items procurring additional to assist with demand.

---

**For the sales team**

For the Sales team, the *Sales by Item* report can be used to quickly identify high performing items in terms of revenue generated.

**Target Audience**

- Sales People

**Example Scenario:** A Salesperson is going to tailor their pitch specific items based on the sales performance. This report can also provide information on lower performing items so sales people can identify upselling or cross-selling.

## Key Performance Indicators (KPIs)

The _Sales by Item_ report includes the following KPIs:

- [**Sales Amount**](#sales-amount)
- [**Sales Quantity**](#sales-quantity)
- [**Cost Amount**](#cost-amount)
- [**Cost Amount Non-Inv**](#cost-amount-non-inv)
- [**Gross Profit**](#gross-profit)
- [**Gross Profit Margin**](#gross-profit-margin)

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

---
### Sales Quantity

The *Sales Quantity* is the total number of items sold within a specific time period.

**Formula**  

*Sales Quantity* is the quantity of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry

---
### Sales Amount

The *Sales Amount* is the actual amount of items sold within a specific time period. This amount represents the net sales amount in local currency, excluding VAT.

**Formula**  

*Sales Amount* is the actual amount of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry

---
### Cost Amount

The *Cost Amount* represents the total cost of goods sold incured by a location within a specific time period.

**Formula**  

*Cost Amount* is the the total cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount*:
- Value Entry

---
### Cost Amount Non-Inv

The *Cost Amount Non-Inv* represents the total cost of non-inventory items by a location within a specific time period. These costs include expenses such as freight costs, shipping costs, marketing expenses, or any other indirect costs associated with sales.

**Formula**  

*Cost Amount Non-Inv* is the the total non-inventory cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount Non-Inv*:
- Value Entry

---
### Gross Profit

The *Gross Profit* shows the difference between the sales revenue and the cost of goods sold for a location within a specifict time period.

**Formula**  

*Gross Profit* = Sales Amount - (Cost Amount + Cost Amount Non-Inv) 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry

---
### Gross Profit Margin

The *Gross Profit Margin* shows the gross profit as a percentage over the sales amount.

**Formula**  

*Gross Profit Margin* = (Gross Profit / Sales Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit Margin*:
- Value Entry


## Data used in the Sales by Item report

Data from the following tables are used on the *Sales by Item* report
- Item
- Item Category
- Value Entry
- Sales Line

## See also