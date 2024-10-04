# Purchases Overview
The _Purchases Overview_ report provides a comprehensive snapshot of an organization’s purchasing activities, offering valuable insights into key metrics such as total purchase amounts, outstanding liabilities, and invoiced purchases. By detailing purchase quantities by location and item category, as well as providing information about vendors, this report aids in financial analysis, budget management, and compliance. It is an essential report for finance and procurement teams, helping them track expenditures, manage budgets, and evaluate vendor performance.


## Target Audience
- CEO, CFO, COO
- Purchasing Managers

## Usage Scenarios
The Purchases Overview report is useful in various scenarios, including:
- **Financial Analysis**: This report helps finance teams track and manage purchasing expenditures.
- **Vendor Management**: This report assists procurement teams in evaluating vendor performance and managing vendor relationships.
- **Budgeting and Forecasting**: This report supports budgeting processes by providing historical purchasing data and trends.

## KPIs
The report shows the following KPIs:
- **Purchase Amount**:
- **Outstanding Amount (excluding VAT)**
- **Amount Received Not Invoiced (excluding VAT)**
- **Invoiced Amount**

### Purchase Amount
This measure represents the total monetary value of all purchases made within a specified period. This metric helps in understanding the overall expenditure on procurement activities.

**Calculation**  
This measure is calculated by summing the total amount of all value entries associated with purchases within the selected time frame.

**Data Sources**  
This measure is calculated from the following tables:
- "Item Ledger Entry"
- "Value Entry"

### Outstanding Amount (excluding VAT)  
The Outstanding Amount measure indicates the total value of purchases that have been ordered but not yet paid for, excluding VAT. This helps in tracking the organization's liabilities.

**Calculation**  
This measure is calculated by summing the value of all unpaid purchase orders, excluding VAT.

**Data Sources**  
This measure is calculated from the following tables:
- "Value Entry"

### Amount Received Not Invoiced (excluding VAT)
The Amount Received Not Invoiced measure shows the value of goods that have been received but not yet invoiced, excluding VAT. It helps in identifying potential discrepancies between received goods and invoiced amounts.

**Calculation**  
This measure is calculated by summing the value of goods received but not yet invoiced on all purchase orders, excluding VAT.

**Data Sources**  
This measure is calculated from the following tables:
- "Value Entry"

### Invoiced Amount
The Invoiced Amount measure represents the total value of purchases that have been invoiced. This metric is crucial for understanding the financial commitments made by the organization.

**Calculation**  
Invoiced Amount is calculated by summing the total value of all purchase invoices within the selected period.

**Data Sources**  
This measure is calculated from the following tables:
- "Value Entry"

## Charts

### Purchase Quantity by Location
This chart displays the total purchase quantity distributed across various locations. It helps in identifying which locations have the highest and lowest purchase quantity.

**Visual Type:**
- Stacked Bar Chart

**Data Source:**
- "Value Entry"
- Location

**Usage:**
- Analyze the distribution of purchase quantities across different locations.
- Identify trends and patterns in purchasing behavior by location.
- Make informed decisions on inventory distribution and logistics.

**Use Cases:**
- **Inventory Management:** Determine which locations require more stock based on purchase quantities.
- **Logistics Planning:** Optimize delivery routes and schedules by understanding high-demand locations.
- **Sales Strategy:** Focus marketing efforts on locations with lower purchase quantities to boost sales.

**Examples:**
- A retail chain analyzing purchase quantities to decide where to open new stores.
- A logistics company planning delivery routes based on purchase data.

**Target Audience:**
- Inventory Managers
- Logistics Coordinators
- Sales and Marketing Teams

### Purchase by Item Category
This chart shows the total purchases categorized by item types. It provides insights into which categories are most frequently purchased.

**Data Sources:**
- "Value Entry"
- Item

**Usage:**
- Understand the purchasing trends across different item categories.
- Identify high-demand categories to optimize stock levels.
- Support strategic planning for procurement.

**Visual Type:**
- Pie Chart / Bar Chart

**Use Cases:**
- **Stock Optimization:** Ensure high-demand items are always in stock.
- **Procurement Planning:** Plan future purchases based on category trends.
- **Sales Analysis:** Identify which categories contribute most to revenue.

**Examples:**
- A supermarket chain analyzing which food categories are most popular.
- An electronics retailer planning inventory based on category sales data.

**Target Audience:**
- Procurement Managers
- Inventory Analysts
- Sales Teams

### Purchase Amounts of Top 5 Vendors

**Description:**
This chart highlights the purchase amounts from the top 5 vendors. It helps in evaluating vendor performance and expenditure distribution.

**Data Source:**
- Purchase Orders Table
- Vendor Table

**Key Metrics:**
- Total Purchase Amount
- Vendor Names

**Usage:**
- Assess the financial impact of top vendors.
- Monitor and compare vendor performance.
- Negotiate better terms with high-volume vendors.

**Visual Type:**
- Bar Chart

**Use Cases:**
- **Vendor Management:** Evaluate and compare the performance of top vendors.
- **Cost Analysis:** Understand expenditure distribution among top vendors.
- **Negotiation:** Use purchase data to negotiate better terms with vendors.

**Examples:**
- A manufacturing company assessing which suppliers provide the most materials.
- A retail chain analyzing spending patterns with top suppliers.

**Target Audience:**
- Procurement Managers
- Financial Analysts
- Vendor Relationship Managers


