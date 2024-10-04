# Home_Sales

# Spark SQL and Parquet Data Processing Exercise

## Summary

This exercise focuses on processing home sales data using Apache Spark. Below is an overview of the steps involved:

1. **Setup Spark**: 
   - Install Spark and Java, then create a Spark session.
   - Read the home sales data from a CSV file into a Spark DataFrame.

2. **Create Temporary View**: 
   - Convert the DataFrame into a temporary SQL table (`home_sales`) to allow SQL queries on the dataset.

3. **Run Queries**: 
   - Calculate the average price of four-bedroom homes sold per year.
   - Query homes with specific characteristics: 3 bedrooms, 3 bathrooms, 2 floors, and at least 2,000 square feet of living space.

4. **Cache Data**: 
   - Cache the `home_sales` table to store it in memory and improve query performance.

5. **Run Cached Query**: 
   - Run a query to calculate the average home price per view rating on the cached data and measure its execution time.

6. **Partition Data**: 
   - Partition the data by `date_built` and save it in Parquet format for optimized storage and access.

7. **Read Parquet Data**: 
   - Load the partitioned Parquet data into a new DataFrame.

8. **Create Temporary Table from Parquet**: 
   - Create a temporary SQL table from the Parquet DataFrame to query it using SQL.

9. **Query Parquet Data**: 
   - Run the query on the Parquet data and compare the execution time to the cached query.

10. **Uncache Data**: 
    - Uncache the `home_sales` table to free up memory when no longer needed.

The goal of the exercise is to practice using Spark for large-scale data processing, including caching, partitioning, and querying with SQL. The comparison of runtime between cached and Parquet queries highlights the performance benefits of caching and partitioning.

## Code Source
- Learning Assistant
- GitHub location: https://github.com/jeffjunohkim/Home_Sales.git