# mysql-project-by-gifted-DHL
data query and databases. more info in readme
-- Create Database Superstore_db;

-- USE Superstore_db;

-- show Tables;

-- select * 
-- from superstore_sales;

-- select `ORDER ID`, Sales superstore_salessuperstore_salessuperstore_table
-- from superstore_sales
-- where Sales > 500;

-- -- select *
-- -- from superstoresales
-- -- limit 10;

-- -- EXERCISE 2

-- select `Order ID`, `Customer Name`, Sales, Profit from superstoresales; 
-- describe superstoresales;
--  select `Order ID`, `Customer Name`, Sales, Profit from superstoresales;
--   select `Order ID`, Sales 
--   from superstoresales
--  where Sales >500
--   LIMIT 10; 
--   select `Order ID`, `Customer Name`, Region
-- from superstoresales
-- where Region = 'West';
--  describe superstoresales;
--  select `Order ID`, Sales
--  from superstoresales
-- order by Sales desc
--  limit 50;
--  
-- --  EXERCISE 6 SORT `CUSTOMER NAME` highest profit only in the West Region. let's see only 100 rows. 
-- select *
-- from superstoresales
-- where Region = 'West'
-- Order by Profit Desc
-- Limit 100;

-- show tables
--  -- EXERCISE 7 TOTAL SALES

-- Select SUM (Sales) As Total_sales
--  from superstoresales;
--  
--  -- use superstore_db;

-- -- VERIFY IMPORTED DATA

-- -- select * from superstore_sales
-- -- limit 10; 

-- -- describe superstore_sales;

-- -- select * from superstore_sales;

-- -- use superstore_db;
-- -- show tables; 

-- -- select database();

-- -- CHECK ROW COUNT (0 means data did not import, >0 data exists but not displaying)

-- -- select count(*) from superstore_sales;

-- -- select * from superstore_sales limit 10;

-- -- commit;

-- -- EXERCISE 1
-- -- select * from superstore_sales limit 10;

-- -- EXERCISE 2 (show order_id, customer name, sales, profit)

-- -- describe superstore_sales;

-- -- select Order_ID, Customer_Name, Sales, Profit from superstore_sales;

-- -- USE BACKTICKS WHEN COLUMN NAMES HAVE SPACES. BACKTICKS IS BELOW YOUR ESC ~`

-- -- select `Order ID`, `Customer Name`, Sales, Profit from superstore_sales; 

-- -- EXERCISE 3 FILTER

-- -- select `Order ID`, Sales 
-- --  from superstore_sales
-- --  where Sales >500
-- --  LIMIT 10; 

-- -- EXERCISE 4 CHECK ORDERS FROM WEST REGION

-- select `Order ID`, `Customer Name`, Region
-- from superstore_sales
-- where Region = 'West';

-- -- describe superstore_sales;

-- -- EXERCISE 5 SORT RESULTS highest sales first

-- -- select `Order ID`, Sales
-- -- from superstore_sales
-- -- order by Sales desc
-- -- limit 50;

-- -- -- EXERCISE 6 SORT CUSTOMER NAME highest profit only in the West Region. let's see only 100 rows. 


-- Describe superstoresales;

-- -- EXERCISE 7 TOTAL SALES
--   select sum(Sales) as total_sales
--  from superstoresales;
--  
--  
--  
--  -- Tasks to be done!
--  -- Show 10 orders with the lowest sales
--  select *
--  From superstoresales
--  Order By Sales ASC
--  Limit 10;
--  
--  -- Count how many orders are from Central region
--  Select Count(*) AS Total_Orders
--  From superstoresales
--  Where `Region` = 'Central';
-- --  Show total profit per Sub-Category
-- Select `Sub-Category`, Sum(`Profit`) AS Total_Profit
-- From superstoresales
-- group by `Sub-Category`
-- order by Total_Profit DESC;

-- -- Show orders with Quantity ≥ 5
-- Select *
-- From superstoresales
-- Where `Quantity` = 5;

-- -- Show top 5 most profitable products
-- Select `Product Name`, sum(`Profit`) AS Total_Profit
-- From superstoresales
-- group by`Product Name`
-- order by Total_Profit DESC
-- Limit 5;

--  
