# Sales by Location (Power BI Report)

The _Sales by Location_ report provides an overview of sales performance broken down by location. It showcases key metrics such as total sales amount, total quantity sold, and cost of goods sold. This information can be further broken down by specific items sold at each location.

This report is targeted towards leadership and management teams to help them track revenue and cost breakdown per location, making it an essential report for any organization that operates across multiple locations.

![Sales by Location screenshot](/business-central/media/sales/sales-by-location.png "Sales by Location - Screenshot")
## What the report shows

The _Sales by Location_ report provides a comprehensive view of the total revenue generated by each location in a bar chart and includes a drill-through table that allows users to view sales breakdowns by location and item in greater detail.

## Use Cases

For the Leadership Team:

The COO of a retail company with multiple warehouse locations wants to know a high-level view of the sales performance of each location to make informed decisions about resource allocation and expansion plans. By using the _Sales by Location report_, the COO can quickly see the total revenue generated by each location and identify any underperforming locations, ensuring that the organization is operating efficiently and effectively across all locations.

**Target Audience**

- CEO
- COO
  
---
For the Management Team:

A Regional Manager responsible who oversees several warehouse locations can track revenue and cost breakdown per location to identify areas for improvement and to adjust sales strategies. By using the _Sales by Location_ report, the manager can quickly see the total sales amount, quantity sold, cost of goods sold, and gross profit for each location. With the drill-through table, the manager can dive deeper into the specific items sold at each location and adjust the product prices accordingly. 

**Target Audience**

- Regional Manager
- Sales Manager


## Key Performance Indicators (KPIs)

The _Sales by Location_ report includes the following KPIs:

- **[Sales Amount](#sales-amount)**  
- **[Sales Quantity](#sales-quantity)**  
- **[Cost Amount](#cost-amount)**  
- **[Cost Amount Non-Inv](#cost-amount-non-inv)**  
- **[Gross Profit](#gross-profit)**  
- **[Gross Profit Margin](#gross-profit-margin)**

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

---
### Sales Amount

The *Sales Amount* represents the total revenue generated by a location from all sales activities within a specific time period.

**Formula**  

*Sales Amount* is the total amount of all value entries related to sales from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry

---
### Sales Quantity

The *Sales Quantity* represents the total quantity sold by a location from all sales activities within a specific time period.

**Formula**  

*Sales Quantity* is the total quantity of all value entries related to sales from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
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

## Data used in the Sales by Location report

Data from the following tables are used on the *Sales by Location* report
- Location
- Item
- Value Entry
- Sales Line

## See also
