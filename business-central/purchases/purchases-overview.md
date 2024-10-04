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

**Data Source(s)**
This measure is calculated from the following tables:
- "Purchase Header"
- "Purchase Line"

### Amount Received Not Invoiced (excluding VAT)
The Amount Received Not Invoiced measure shows the value of goods that have been received but not yet invoiced, excluding VAT. It helps in identifying potential discrepancies between received goods and invoiced amounts.

**Calculation**  
This measure is calculated by summing the value of goods received but not yet invoiced on all purchase orders, excluding VAT.

**Data Source(s)**
This measure is calculated from the following tables:
- "Purchase Header"
- "Purchase Line"

### Invoiced Amount
The Invoiced Amount measure represents the total value of purchases that have been invoiced. This metric is crucial for understanding the financial commitments made by the organization.

**Calculation**  
Invoiced Amount is calculated by summing the total value of all purchase invoices within the selected period.

**Data Source(s)**  
TODO: To be added
