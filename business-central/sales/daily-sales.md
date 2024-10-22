# Daily Sales (Power BI Report)

The _Daily Sales_ report gives a clear picture of your organization's sales activities over specific days. This report can showcase the days with a higher volume of sales. This can be broken down further to view variations across different years, quarters or months to identify trends with sales.

This report is meant for sales teams to track sales across different dates and periods.

![Daily Sales screenshot](/business-central/media/sales/sales-daily-sales.png "Daily Sales - Screenshot")

## What the report shows

The *Daily Sales* report showcases a daily sales figure spread across each indiviudal date. This can showcase high and low demand days. This report visuals this data in both a matrix view and a standard table view. The figures can also be drilled into opening up the Sales drill-through page.


## Use Cases for Daily Sales

**For the leadership team**

For the leadership team, the *Daily Sales* report can be used to idenfity the sales performance on a day by day basis to make more informed decisions. 

**Target Audience**

- Executives

**Example Scenario:** You are an executive and want to view detailed sales information on a day by day basis.

---

**For the management team**

For the management team, the *Daily Sales* can be used to monitor the daily sales overall sales performance.

**Target Audience**

- Sales Managers

**Example Scenario:** As a sales manager you want to view the daily sales statistics of a specific sales people.

---

**For the sales team**

For the Sales team, the *Daily Sales* report can be used to gain a clearer understanding of customer metrics and identify any stands out.  

**Target Audience**

- Sales People

**Example Scenario:** You are a Salesperson who is going to a customer sites and wants to identify recent trends for this customer and see what days they usually purchase items.




## Key Performance Indicators (KPIs)

The _Daily Sales_ report includes the following KPIs:

- **Sales Quantity**
- **Sales Amount**
- **Cost Amount**
- **Gross Profit**
- **Gross Profit Margin**

Below, you can learn more about what each KPI means, how it is calculated, and what data was used in the calculations.

---
### Sales Quantity

The *Sales Quantity* is the total number of items sold within a specific time period.

**Formula**  

*Sales Quantity* is the quantity of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Quantity*:
- Value Entry
- Sales Line

---
### Sales Amount

The *Sales Amount* is the actual amount of items sold within a specific time period. This amount represents the net sales amount in local currency, excluding VAT.

**Formula**  

*Sales Amount* is the actual amount of all value entries related to sales for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Sales Amount*:
- Value Entry
- Sales Line

---
### Cost Amount

The *Cost Amount* represents the total cost of goods sold incured by a location within a specific time period.

**Formula**  

*Cost Amount* is the the total cost of all sales value entries from the location for the selected timeframe.

**Data Sources**

Data from the following tables are used to calculate the *Cost Amount*:
- Value Entry
- Sales Line

---
### Gross Profit

The *Gross Profit* shows the difference between the sales revenue and the cost of goods sold for a location within a specifict time period.

**Formula**  

*Gross Profit* = Sales Amount - (Cost Amount + Cost Amount Non-Inv) 

**Data Sources**

Data from the following tables are used to calculate the *Gross Profit*:
- Value Entry
- Sales Line

---
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