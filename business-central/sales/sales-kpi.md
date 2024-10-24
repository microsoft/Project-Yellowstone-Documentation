# Sales App KPIs


## Key Performance Indicators (KPIs)


### Sales Table
**Counters**
- [No. of Distinct Items](#no-of-distinct-items)
- [No. of Outstanding Sales Orders](#no-of-outstanding-sales-orders)
- [No. of Posted Sales Invoices](#no-of-posted-sales-invoices)
- [No. of Shipped Not Invoiced Sales](#no-of-shipped-not-invoiced-sales)

**Sales Measures**
- **Invoiced**
    - [Invoiced Amount](#invoiced-amount)
    - [Invoiced Quantity](#invoiced-quantity)
- **Outstanding**
    - [Outstanding Amount](#outstanding-amount)
    - [Outstanding Quantity](#outstanding-quantity)
- **Shipped Not Invoiced**
    - [Shipped Not Invoiced Amount](#shipped-not-invoiced-amount)
    - [Shipped Not Invoiced Quantity](#shipped-not-invoiced-quantity)
- [Cost Amount](#cost-amount)
- [Cost Amount Non-Inv](#cost-amount-non-inv)
- [Gross Profit](#gross-profit)
- [Gross Profit Margin](#gross-profit-margin)
- [Sales Amount](#sales-amount)
- [Sales Quantity](#sales-quantity)

#### Invoiced Amount
**Formula**  
Sum of Sales Amount column from the Sales table where Source Type = Value Entries Invoiced.

**Data Sources**
- Value Entries

#### Invoiced Quantity
**Formula**  
Sum of Sales Qty. (Base) column from the Sales table. where Source Type = Value Entries Invoiced.

**Data Sources**
- Value Entries

#### Outstanding Amount
**Formula**  
Sum of Sales Amount column from the Sales table where Source Type = Sales Order Outstanding.

**Data Sources**
- Sales Line

#### Outstanding Quantity
**Formula**  
Sum of Sales Qty. (Base) column from the Sales table. where Source Type = Sales Order Outstanding.

**Data Sources**
- Sales Line

#### Shipped Not Invoiced Amount
**Formula**  
Sum of Sales Amount column from the Sales table where Source Type = Sales Order Shipped Not Invoiced.

**Data Sources**
- Sales Line

#### Shipped Not Invoiced Quantity
**Formula**  
Sum of Sales Qty. (Base) column from the Sales table. where Source Type = Sales Order Shipped Not Invoiced.

**Data Sources**
- Sales Line

### Sales Budget Table
**Budget Measures**
- [Budget Amount](#budget-amount)
- [Budget Amount Variance](#budget-amount-variance) 
- [Budget Amount Variance %](#budget-amount-variance-percent)
- [Budget Quantity](#budget-quantity)
- [Budget Quantity Variance](#budget-quantity-variance)
- [Budget Quantity Variance %](#budget-quantity-variance-percent)


### Customer Table
**Customer Measures**
- [No. of Customers](#no-of-customers)
- [No. of Lost Customers](#no-of-lost-customers)
- [No. of New Customers](#no-of-new-customers)
- No. of Recovered Customers
- No. of Returning Customers
- Sales Lost Customers (12M)
- Sales New Customers
- Sales Recovered Customers
- Sales Returning Customers

#### No. of Customers
**Formula**  
Distinct count of Customer No. column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

#### No. of Lost Customers
**Formula**  
This measure calculates the number of customers who have been "lost" within the current date selection. It first determines the latest date in the selection, prepares a table of customers and their associated "lost" dates, and then filters out the customers whose lost date falls within the selected date range. Finally, it counts the rows in this filtered table to get the number of lost customers.

**Data Sources**
- Value Entries
- Sales Line


#### No. of New Customers
**Formula**  
This measure identifies and counts new customers by finding the date of their first purchase and ensures that only customers with first purchase dates within the current date selection are included.

**Data Sources**
- Value Entries
- Sales Line

#### No. of Recovered Customers
**Formula**  
This measure identifies calculates the number of customers who were temporarily lost (stopped purchasing) but later made a new purchase. It first identifies customers who had a "lost" date before the selected date range, then determines which customers made a new purchase within the current period. The measure filters and counts only those customers whose new purchase occurred after their lost date, returning the total number of recovered customers.

**Data Sources**
- Value Entries
- Sales Line










#### Budget Amount
**Formula**  
Sum of Sales Amount column from the Sales Budget table.

**Data Sources**
- Item Budget Entries

#### Budget Amount Variance
**Formula**  
[Sales Amount] - [Budget Amount]

**Data Sources**
- Item Budget Entries
- Sales Lines
- Value Entries

#### Budget Amount Variance Percent
**Formula**  
[Budget Amount Variance] - [Budget Amount]

**Data Sources**
- Item Budget Entries
- Sales Lines
- Value Entries

#### Budget Quantity
**Formula**  
Sum of Quantity column from the Sales Budget table.

**Data Sources**
- Item Budget Entries

#### Budget Quantity Variance
**Formula**  
[Sales Quantity] - [Budget Quantity]

**Data Sources**
- Item Budget Entries
- Sales Lines
- Value Entries

#### Budget Quantity Variance Percent
**Formula**  
[Budget Quantity Variance] - [Budget Quantity]

**Data Sources**
- Item Budget Entries
- Sales Lines
- Value Entries

----
#### No. of Distinct Items
**Formula**  
Distinct count of Item No. column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

#### No. of Outstanding Sales Orders
**Formula**  
Distinct count of Document No. column from the Sales table where Document Type = Order and Source Type = Sales Order Outstanding.

**Data Sources**
- Value Entries
- Sales Line

#### No. of Posted Sales Invoices
**Formula**  
Distinct count of Document No. column from the Sales table where Document Type = Sales Invoice and Source Type = Value Entries Invoiced.

**Data Sources**
- Value Entries
- Sales Line

#### No. of Shipped Not Invoiced Sales
**Formula**  
Distinct count of Document No. column from the Sales table where Document Type = Order and Source Type = Sales Order Shipped Not Invoiced.

**Data Sources**
- Value Entries
- Sales Line

----

#### Cost Amount
**Formula**  
Sum of Cost Amt. (LCY) column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

#### Cost Amount Non-Inv
**Formula**  
Sum of Cost Amt. Non-Invtbl. (LCY) column from the Sales table.

**Data Sources**
- Value Entries

#### Gross Profit
**Formula**  
[Sales Amount] - [Cost Amount] - [Cost Amount Non-Inv]

**Data Sources**
- Value Entries
- Sales Line

#### Gross Profit Margin
**Formula**  
[Gross Profit] / [Sales Amount]

**Data Sources**
- Value Entries
- Sales Line

#### Sales Amount
**Formula**  
Sum of Sales Amt. (LCY) column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line

#### Sales Quantity
**Formula**  
Sum of Sales Qty. (Base) column from the Sales table.

**Data Sources**
- Value Entries
- Sales Line
---

## See also