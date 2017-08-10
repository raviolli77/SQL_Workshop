# Database: Northwind
(go to Ravi's MySQL Workshop repository, scroll down to find the Northwind dataset, download the zip, then in *MySQL Workbench*: File --> Run SQL Script for northwind.sql 
and northwind_data.sql)

1. From the Orders table:
	a. Show table with recipient's name, city, state, and shipping_fee 
	b. Ordered by shipping_fee, most expensive at the top 
2. From the Orders table:
	a. Show a table with state and sum of all shipping_fee for that state 
		i. Group that individual entries by state 
	b. Order by shipping_fee, most money at the top