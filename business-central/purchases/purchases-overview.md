# Purchase Overview (Power BI report)

The _Purchases Overview_ report gives a clear picture of your organization's purchasing activities. It highlights important metrics like total purchase amounts, outstanding liabilities, and invoiced purchases. By breaking down purchase quantities by location and item category, and providing vendor information, this report helps with financial analysis, budget management, and compliance. 

This report is meant for finance and procurement teams to track spending, manage budgets, and evaluate vendor performance.

:::image type="content" source="media/powerbi/powerbi-purchase-purchase-overview.png" alt-text="Screenshot of the Purchase Overview Power BI report" lightbox="media/powerbi/powerbi-purchase-purchase-overview.png":::

## What the report shows

The *Purchase Overview* reports shows ...


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

The *Total Purchase Amount* KPI is important because... (insert text here) This KPI shows the total value of all purchases made within a specific period, helping you understand overall procurement spending.

**Formula**  

*Total Purchase Amount* = sum of the total amount of all value entries related to purchases within the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Total Purchase Amount* KPI:
- "Item Ledger Entry"
- "Value Entry"


### Outstanding Amount (excluding VAT)
This KPI indicates the total value of purchases ordered but not yet paid for, excluding VAT. It helps track your organization's liabilities.

**Calculation**  
By summing the value of all unpaid purchase orders, excluding VAT.

**Data Sources**  
- "Value Entry"

### Amount Received but Not Invoiced (excluding VAT)
This KPI shows the value of goods received but not yet invoiced, excluding VAT. It helps identify discrepancies between received goods and invoiced amounts.

**Calculation**  
By summing the value of goods received but not yet invoiced on all purchase orders, excluding VAT.

**Data Sources**  
- "Value Entry"

### Invoiced Amount
This KPI represents the total value of purchases that have been invoiced, crucial for understanding your financial commitments.

**Calculation**  
By summing the total value of all purchase invoices within the selected period.

**Data Sources**  
- "Value Entry"

## Visual Insights

### Purchase Quantity by Location
This chart shows the total purchase quantity across different locations, helping you see which locations have the highest and lowest purchase quantities.

**Use Cases:**
- **Inventory Management:** Determine which locations need more stock.
- **Purchasing Trends:** Identify trends and patterns in purchasing behavior by location.
- **Logistics Improvement:** Make informed decisions on inventory distribution and logistics.

**Chart Type:**
- Stacked Bar Chart

**Data Sources:**
- "Value Entry"
- Location

### Purchase Quantity by Item Category
This chart displays total purchases by item type, providing insights into the most frequently purchased categories.

**Use Cases:**
- **Stock Optimization:** Ensure high-demand items are always in stock.
- **Item Analysis:** Understand purchasing trends across different item categories.
- **Procurement Planning:** Support strategic procurement planning.

**Chart Type:**
- Pie Chart

**Data Sources:**
- "Value Entry"
- Item

### Purchase Amounts of Top 5 Vendors
This chart highlights the purchase amounts from the top 5 vendors, helping you evaluate vendor performance and expenditure distribution.

**Use Cases:**
- **Vendor Management:** Compare the performance of top vendors.
- **Cost Analysis:** Understand how spending is distributed among top vendors.
- **Negotiation:** Use purchase data to negotiate better terms with vendors.

**Chart Type:**
- Stacked Bar Chart

**Data Sources:**
- "Value Entry"
- Vendor


## Data used in the Purchases Overview report

Data from the following tables are used on the *Purchases Overview* report
- "Item Ledger Entry"
- "Value Entry"


## See also
