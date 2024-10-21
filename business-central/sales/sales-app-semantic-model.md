# Sales App Semantic Model

The Sales semantic model is organized in a  [Star Schema Model](https://learn.microsoft.com/en-us/power-bi/guidance/star-schema#star-schema-overview). 

The Fact tables contains information about individual transactions from sources such as sales orders, posted sales invoices and posted credit memos. Dimension tables provide additional context and attributes to the transactional data, such as customer and product information.

## Fact Tables
Fact tables store transactional data and support summarizations such as SUM, AVG, COUNT and more. There are two fact tables in the Power BI Sales app: 
- [Sales](#sales)
- [Sales Budget](#sales-budget)

### Sales
Source table(s):
- Value Entries
- Sales Lines

Sales Lines are broken down into Shipped Not Invoiced and Outstanding Sales Lines. The Source Type field allows for filtering by these sources. 

##### Table Definition

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Date | Order Date / Posting Date | Order Date is used for data from Sales Lines. Posting Date is used for data from Value Entries. |
| Document No. |  Document No. | Specifies the documents no. |
| Document Type |  Document Type | Specifies the documents type |
| Entry No. |  Entry No. / Sales Line No. | When reporting on Value Entries this represents the value entry no. When reporting on sales lines this represents the sales line no. |
| Entry Type |  Entry Type | When reporting on Value Entries this represents the entry type of the value entry. When reporting on sales lines the value reads "Sales Line" |
| Source Type |  - | A delineating field used to define the source table of the record. |


### Sales Budget
Source table(s):
- Item Budget Entries

##### Table Definition

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Budget Name | Budget Name | Specifies the name of the budget |
| Date |  Date | Specifies the date for the budget entry |
| Entry No. |  Entry No. | The unique no. of the specific budget entry |

## Dimension Tables
In the star schema model, the dimension tables are used to support the data model and allow filtering and grouping.

- [Customer](#customer)
- [Item](#item)
- [Location](#location)
- [Salesperson](#salesperson)

### Customer
Source table(s):
- Customer

##### Table Definition

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
Source table(s):
- Item
- Item Category

##### Table Definition

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
Source table(s):
- Location

##### Table Definition

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Location Code | Code | Specifies the Code of the Location |
| Location Name |  Name | Specifices the Name of the Location |

### Salesperson
Source table(s):
- Salesperson/Purchaser

##### Table Definition

| Power BI Field Name | Business Central Field Name | Description |
| ------ | -------------- | ---------- |
| Salesperson Code | Code | Specifies the Salespersons Code |
| Salesperson Name |  Name | Specifies the Salespersons Name |