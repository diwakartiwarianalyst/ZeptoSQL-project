# Zepto SQL Data Analysis

## About
This project is based on a Zepto dataset where I explored product-level data using SQL. The main focus was to clean the data and extract useful insights related to pricing, discounts, and stock availability.

## Tools Used
- MySQL

## Database Setup
- Created a database named `zeptodatabase`
- Built a table `zepto` with product details like category, price, discount, stock, and weight

## Work Done

### Data Exploration
- Checked total number of records  
- Identified null values in the dataset  
- Found unique product categories  
- Analyzed stock availability (in stock vs out of stock)  
- Checked duplicate product names  

### Data Cleaning
- Identified products with 0 price  
- Converted price values from paisa to rupees  

### Analysis & Insights

- Found top 10 products with highest discount  
- Identified expensive products that are out of stock  
- Calculated estimated revenue category-wise  
- Filtered products based on price and discount conditions  
- Found top categories with highest average discount  
- Calculated price per gram for better comparison  
- Grouped products into Low, Medium, and Bulk based on weight  

## Sample Query

```sql
SELECT name, mrp, discountPercent
FROM zepto
ORDER BY discountPercent DESC
LIMIT 10;
