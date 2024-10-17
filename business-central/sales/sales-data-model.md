# Sales Data Model

The Sales Data model is built on the premise of a [Star Schema Model](https://learn.microsoft.com/en-us/power-bi/guidance/star-schema#star-schema-overview). This has multiple Fact and Dimension tables to create the entire model available in the Power BI Sales App.

## Fact Tables
The fact tables store the transactional data that is pulled into Power BI from Business Central. There is two primary fact tables in the Power BI Sales app being the Sales and Sales Budget tables.

### Sales
The Sales table in Power BI pulls data from two separate tables in Business Central
- Value Entries
- Sales Lines

Sales Lines are then broken up into Sales Lines that are Shipped Not Invoiced and Outstanding Sales Lines. This allows users to filter to specific Sales Metrics using the Source Type.

The following sections provide an overview of the **Sales** fact table:

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Date | Order Date/Posting Date | Order Date is used from the Sales Line and Posting Date is used from the Value Entries. This is linked to the Date table in Power BI to allow filtering on specifc date values. |
| Document No. |  Document No. | Specifies the documents no. |
| Document Type |  Document Type | Specifies the documents type |
| Entry No. |  Entry No. | Used for reporting on Value Entries, this outlines the unique no. of the value entry. When reporting on sales lines, this will show the sales line no. |
| Entry Type |  Entry Type | Used for reporting on Value Entries, this outlines the entry type of the value entry. When reporting on sales lines, this will show the type as "Sales Line" |
| Source Type |  - | A unqiue field added in Power BI used to differentiate the different Sales Type used in Power BI. This can be Sales Order (Outstanding), Sales Orders (Shipped Not Invoiced) or Value Entries (Invoiced). This is editable through the data model settings updating the parameter |


### Sales Budgets
The Sales Budget table in Power BI pulls data from the below table in Business Central
- Item Budget Entries

The following sections provide an overview of the **Sales Budget** fact table:

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Budget Name | Budget Name | Specifies the name of the budget |
| Date |  Date | Specifies the date for the budget entry |
| Entry No. |  Entry No. | The unique no. of the specific budget entry |

## Dimension Tables
In the star schema model, the dimension tables are used to support the data model and allow filtering and grouping.

### Customer
The Customer table in Power BI pulls data from the below table in Business Central
- Customer

The following sections provide an overview of the **Customer** dimension table:

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Customer No. | No. | Specifies the Customer No. |
| Customer Name |  Name | Specifies the Customer Name |
| Customer No. and Name |  - | Combination of Customer No. and Customer Name done inside of Power BI |
| Address | Address | Specifies the Address |
| Address 2 |  Address 2 | Specifies the secondary Address details |
| City |  City | Specifies the City |
| Post Code | Post Code | Specifies the address Postal Code |
| County |  County | Specifies the state |
| Country/Region Code |  Country/Region Code | Specifies the country/region of the address |
| Customer Posting Group | Customer Posting Group | Specifies the posting group |
| Customer Price Group |  Customer Price Group | Specifies the price group |
| Customer Disc. Group |  Customer Disc Group | Specifies the discount group |

### Item
The Item table in Power BI pulls data from the below tables in Business Central
- Item
- Item Category

The following sections provide an overview of the **Item** dimension table:

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Item No. | No. | Specifies the Items No. |
| Item Name |  Description | Specifies the Items Description |
| Item No. and Name |  - | Combination of Item No. and Item Name done inside of Power BI |
| Base Unit of Measure | Base Unit of Measure | Specifies the Base Unit of Measure |
| Unit Cost |  Unit Cost | Specifies the Unit Cost |
| Inventory Posting Group | Inventory Posting Group | Specifies the Inventory Posting Group |
| Item Category Code |  Code | Specifies the Item Category |
| Item Category Description |  Description | Specifies the description of the Item Category the item belongs to |

### Location
The Location table in Power BI pulls data from the below table in Business Central
- Location

The following sections provide an overview of the **Location** dimension table:

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Location Code | Code | Specifies the Code of the Location |
| Location Name |  Name | Specifices the Name of the Location |

### Salesperson
The Customer table in Power BI pulls data from the below table in Business Central
- Salesperson/Purchaser

The following sections provide an overview of the **Salesperon** dimension table:

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Salesperson Code | Code | Specifies the Salespersons Code |
| Salesperson Name |  Name | Specifies the Salespersons Name |
