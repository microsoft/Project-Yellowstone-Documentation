# Purchase Overview (Power BI report)

The _Purchases Overview_ report gives a clear picture of your organization's purchasing activities. It highlights important metrics like total purchase amounts, outstanding liabilities, and invoiced purchases.

This report is meant for finance and purchasing teams to track spending, manage budgets, and evaluate vendor performance.

**TODO: Insert screenshot here**

## What the report shows

The *Purchase Overview* reports provides a snapshot of purchasing activities within the organization.

## How to use the Purchases Overview report

The _Purchases Overview_ report can be used in various ways, such as 
- **Financial Analysis**: Helps finance teams track and manage purchasing expenses.
- **Vendor Management**: Assists procurement teams in evaluating and managing vendor relationships.
- **Budgeting and Forecasting**: Supports budgeting by providing historical purchasing data and trends.


## Key Performance Indicators (KPIs)
The _Purchases Overview_ report includes the following KPIs:

- **Total Purchase Amount**
- **Outstanding Amount (excluding VAT)**
- **Amount Received but Not Invoiced (excluding VAT)**
- **Invoiced Amount**

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

[!INCLUDE[powerbi-tip-track-kpis](includes/powerbi-tip-track-kpis.md)]

### Total Purchase Amount

The *Total Purchase Amount* KPI is important for understading the overall spending on all purchasing activities. This KPI shows the total amount of all purchases made within a specific period.

**Formula**  

*Total Purchase Amount* is the sum of the amount of all value entries related to purchases within the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Total Purchase Amount* KPI:
- Item Ledger Entry
- Value Entry

### Outstanding Amount
The _Outstanding Amount_ KPI helps with tracking the liabilities within the organization. This KPI indicates the total value of purchase orders but not yet paid for, excluding VAT amount.

**Calculation**  

*Outstanding Amount* is the sum of the amount of all unpaid purchase orders, excluding VAT.

**Data Sources**

Data from the following table is used to calculate the *Outstanding Amount* KPI:
- Value Entry

### Amount Received but Not Invoiced
The *Amount Received but Not Invoiced* KPI highlights the discrepancies between received goods and invoiced amounts. This KPI shows the value of goods received but not yet invoiced, excluding VAT.

**Calculation**  

*Amount Received but Not Invoiced* is the sum of the value of goods received but not yet invoiced on all purchase orders, excluding VAT.

**Data Sources**

Data from the following table is used to calculate the *Amount Received but Not Invoiced* KPI:
- Value Entry

### Invoiced Amount
The *Invoiced Amount* is important for understanding the actual spending on all purchasing activities within the organization. This KPI represents the total value of all purchases that have been invoiced.

**Calculation**  

*Invoiced Amount* is the sum of the value of all purchase invoices within the selected timeframe.

**Data Sources**

Data from the following table is used to calculate the *Invoiced Amount* KPI:
- Value Entry

## Visual Insights

### Purchase Quantity by Location
This chart shows the total purchase quantity across different locations, helping you see which locations have the highest and lowest purchase quantities.

**Data Sources**

Data from the following tables are used for this chart:
- Value Entry
- Location

### Purchase Quantity by Item Category
This chart displays total purchases by item type, providing insights into the most frequently purchased item categories.

**Data Sources**

Data from the following tables are used for this chart:
- Value Entry
- Item

### Purchase Amounts of Top 5 Vendors
This chart highlights the purchase amounts from the top 5 vendors, helping you evaluate vendor performance and expenditure distribution.

**Data Sources**

Data from the following table is used for this chart:
- Value Entry

## Data used in the Purchases Overview report
Data from the following tables are used on the *Purchases Overview* report
- Item Ledger Entry
- Value Entry
- Item
- Location


## See also
