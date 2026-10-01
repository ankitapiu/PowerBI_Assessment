 Data Model
 
- Implemented Star Schema
- FactSales as central fact table
- DimDate, DimProduct,dim_agent used as dimensions
- One-to-many relationships
 
Reason:
Star Schema improves model performance and DAX efficiency.

 DAX approach for the hardest measure

APE Rolling 3 Months = CALCULATE(SUM(fact_sales[ape_usd]),DATESINPERIOD(dim_date[date],MAX(dim_date[date]),-3,MONTH))

### Improvements With More Time Example:

Dax complex codes
Incremental Refresh
Calculation Groups 
Additional KPI drillthrough pages 
Performance optimization using Aggregations 
Enhanced mobile layout
