# Sales App KPIs


## Key Performance Indicators (KPIs)


### Sales
#### Counters
- No. of Distinct Items
- No. of Outstanding Sales Orders
- No. of Posted Sales Invoices
- No. of Shipped Not Invoiced Sales

#### Sales Measures
- Cost Amount
- Cost Amount Non-Inv
- Gross Profit
- Gross Profit Margin
- Sales Amount
- Sales Quantity

##### Invoiced
- Invoiced Amount
- Invoiced Quantity

##### Outstanding
- Outstanding Amount
- Outstanding Quantity

##### Shipped Not Invoiced
- Shipped Not Invoiced Amount
- Shipped Not Invoiced Quantity

---
### Sales Budget
#### Budget Measures
- Budget Amount
- Budget Amount Variance
- Budget Amount Variance %
- Budget Quantity
- Budget Quantity Variance
- Budget Quantity Variance %

---
### Customer
#### Customer Measures
- No. of Customers
- No. of Lost Customers
- No. of New Customers
- No. of Recovered Customers
- No. of Returning Customers
- Sales Lost Customers (12M)
- Sales New Customers
- Sales Recovered Customers
- Sales Returning Customers

The *Sales Amount* is the actual amount of items sold within a specific time period. This amount represents the net sales amount in local currency, excluding VAT.

**Formula**  

*Sales Amount* is the actual amount of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry
- Sales Line

### Sales Quantity

The *Sales Quantity* is the total number of items sold within a specific time period.

**Formula**  

*Sales Quantity* is the quantity of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry
- Sales Line


### Cost Amount

The *Cost Amount* represents the total cost of goods sold incured by a location within a specific time period.

**Formula**  

*Cost Amount* is the the total cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount*:
- Value Entry
- Sales Line

### Gross Profit

The *Gross Profit* shows the difference between the sales revenue and the cost of goods sold for a location within a specifict time period.

**Formula**  

*Gross Profit* = Sales Amount - (Cost Amount + Cost Amount Non-Inv) 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry
- Sales Line

### Gross Profit Margin

The *Gross Profit Margin* shows the gross profit as a percentage over the sales amount.

**Formula**  

*Gross Profit Margin* = (Gross Profit / Sales Amount) x 100

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit Margin*:
- Value Entry
- Sales Line


## Data used in the Daily Sales report

Data from the following tables are used on the *Daily Sales* report
- Value Entry
- Sales Line
- Item


## See also