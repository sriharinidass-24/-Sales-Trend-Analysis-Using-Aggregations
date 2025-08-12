# Task 6: Sales Trend Analysis Using Aggregations

## Objective
Analyze monthly revenue and order volume from the sales dataset using SQL aggregation functions.

## Tools Used
- **SQLite** (for running SQL queries)

## Dataset Description
The dataset `sales_data_cleaned` contains cleaned sales transaction records.  
Main columns used:
- `sale_date` – Date of sale in DD-MM-YYYY format  
- `product_category` – Category of the sold product  
- `sales_amount` – Revenue generated from the sale  

## Steps Taken
1. Converted `sale_date` into proper `year` and `month` values using `strftime()` and `substr()` for extraction.  
2. Grouped the results by **year**, **month**, and **product category**.  
3. Calculated:
   - **Total Revenue** → `SUM(sales_amount)`  
   - **Total Sales Records** → `COUNT(*)`  
   - **Average Sale Value** → `SUM(sales_amount) / COUNT(*)`  
4. Ordered the results by year, month, and category for better trend analysis.
