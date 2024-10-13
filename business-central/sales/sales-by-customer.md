# Sales by Customer (Power BI Report)

The _Sales by Customer_ report gives a clear picture of your organization's customers and their sales activities. It highlights key metrics against each Customer such as Sales Amount and Quantities along with the Costs associated. This can be broken down further by the specific items that are being sold per customer to identify key trends. By breaking down Sales by Customer, this report provides clear information on your organizations customers.

This report is meant for all users to identifiy key customers and customers that may be purchasing less than expected. U

![Sales by Customer screenshot](/business-central/media/sales/sales-by-customer.png "Sales by Customer - Screenshot")

## What the report shows

The *Sales by Customer* reports shows outlines a comprehensive view of the total sales generated. This is viewable in both a barchart and matrix view. Each visual links to the Sales drill-through page to further breakdown the information.


## Use Cases

**For the leadership team**

For the leadership team, the *Sales by Customer* report provides insights into the top customers generating revenue for the company. 

**Target Audience**

- CFO

**Example Scenario:** The CFO wants to see a list of top customers generating revenue for the company. Additionally they want to be able to identify which customers are generating the most revenue and how much each customer is contributing to the company's overall revenue.customer frequently orders vs items they are not ordering.

---

**For the management team**

For the management team, the *Sales by Customer* report can be used to monitor performance of the sales teams in terms of customer acquistion and longevity.

**Target Audience**

- Sales Manager
- Business Development Manager

**Example Scenario:** The sales management team want to identify which salespeople are acquring new customers and providing existing customers with the best offering.

---

**For the sales team**

For the Sales team, the *Sales by Customer* report can be used to track their customers and identify their top performing customers. 

**Target Audience**

- Sales Representative

**Example Scenario:** A Salesperson wants to be able to review and identify opportunities for upselling or cross-selling to a specific customer.

## Key Performance Indicators (KPIs)

The _Sales by Customer_ report includes the following KPIs:

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


## Data used in the Sales by Customer report

Data from the following tables are used on the *Sales by Customer* report
- Customer
- Item
- Value Entry
- Sales Line

## See also