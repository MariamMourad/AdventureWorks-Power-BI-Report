# AdventureWorks Power BI Report
- Data Source: 
https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15&tabs=ssms

Conductivity Mode => DirectQuery

##Tables:
Sales.SalesOrderHeader
Sales.SalesOrderDetail
Sales.vSalesPerson (view)
Sales.SalesTerritory
Purchasing.ShipMethod
Production.Product
Production.ProductSubcategory
Production.ProductCategory

Status (Add based on ufnGetSalesOrderStatusText function)
Dates (DAX)

-Rename Tables, columns
-Remove unused columns 

-one table (Merge M Language)
Production.Product
Production.ProductSubcategory
Production.ProductCategory

Contains: PorductID, Product, SubCategory, Category

Solve TotalDue, Tax and Fright by Power Query

##Modelig:

- Star Schema 
- Product Hierarchy


- line chart vs. counts (USERELATIONSHIP)
orderdate
shipdate
duedate


##Measures
- Number of Orders Measure 
- Total SubTotal Measure 
- Total Tax Measure 
- Total Freight Measure 
- Total Due Measure 
- Number of Qty

create DAX table that contains all measures

##Visuals: (Use Measures)

- Drill Down
- Drill Through 
- Tooltip page

- Number of Orders Card
- Total SubTotal Card
- Total Tax Card
- Total Freight Card
- Total Due Card

- Number of Orders by OrderDate vs. ShipDate vs. DueDate
- Number of Orders by Status
- Number of Orders by Shipmethod
- Number of Orders by Category, SubCategory, Product
- Number of Orders by FlagOnlineOffline
- Number of Orders vs. TotalDue by Territory
- Top 10 Sales Perosns (Number of Orders and Total Amount) (Top N Filter)
