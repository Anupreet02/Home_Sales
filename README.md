# Home_Sales

The  Home_Sales_colab.ipynb is the solved 

* [ ] **Overview**

This project involves analyzing home sales data using PySpark SQL functions. The goal is to explore insights from the data and demonstrate performance optimization techniques such as caching and partitioning. Below is an outline of the tasks and their purposes.

1. **Data Import and Table Creation**

* Import the required PySpark SQL functions for analysis.
* Read the home_sales_revised.csv file into a Spark DataFrame.
* Create a temporary table named home_sales for SQL querying.

3. **Analytical Queries**

* 3.1 Average Price for Four-Bedroom Houses by Year
* Determine the average price for four-bedroom houses sold each year.
* Round the results to two decimal places.

3.2 Average Price for 3-Bedroom, 3-Bathroom Homes by Year Built

* Calculate the average price of homes with three bedrooms and three bathrooms for each year they were built.
* Round the results to two decimal places.

3.3 Average Price for Specific 3-Bedroom Homes

* Calculate the average price of homes with the following criteria:
* Three bedrooms
* Three bathrooms
* Two floors
* Greater than or equal to 2,000 square feet
* Round the results to two decimal places.

3.4 Average Price per View Rating

* Determine the average price of homes per "view" rating where the average home price is greater than or equal to $350,000.
* Record the runtime of the query and round the results to two decimal places.

4. **Caching**

* Cache the home_sales temporary table to improve performance.
* Verify that the table is cached.
* Re-run the query from 3.4 using cached data and compare the runtime with the uncached version.

5. **Partitioning and Parquet**

* Partition the home sales data by the date_built field and save it in Parquet format.
* Create a temporary table for the Parquet data.
* Re-run the query from 3.4 on the partitioned data and compare its runtime to previous versions.

6. **Uncaching**

* Uncache the home_sales temporary table.
* Verify that the table is no longer cached

7. **Insights**

* This project provides insights into:
* Home pricing trends based on number of bedrooms and bathrooms.
* The effect of specific features (e.g., size, floors) on home pricing.
* The relationship between "view" ratings and average home prices.
* Performance Optimization
* Techniques Used
* Caching: Improved query runtime by storing data in memory.
* Partitioning: Enhanced performance for queries on large datasets by saving data in Parquet format partitioned by date_built.

## Summary

This project involves analyzing home sales data using PySpark SQL functions to derive insights and demonstrate performance optimization techniques. Key tasks include querying home prices based on specific criteria, improving query performance with caching and partitioning, and documenting results for future use.
