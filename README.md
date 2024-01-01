# Home_Sales

# Spark SQL Tasks README

This README provides an overview of the Spark SQL tasks performed using Apache Spark.

## Prerequisites

Make sure you have the following prerequisites installed:

- Apache Spark
- Python (if running PySpark scripts)

## Tasks

### 1. Read Data from AWS S3

- Imported `findspark` and initialized it.
- Imported necessary Spark packages and set up a Spark session.
- Read data from an AWS S3 bucket into a DataFrame.

### 2. Create a Temporary View

- Created a temporary view of the DataFrame for Spark SQL queries.

### 3. Average Price for Four Bedroom Houses

- Calculated the average price for a four-bedroom house sold in each year, rounded to two decimal places.

### 4. Average Price for Three Bedroom, Three Bathroom Houses

- Calculated the average price of a home for each year it was built that has 3 bedrooms and 3 bathrooms, rounded to two decimal places.

### 5. Average Price for Three Bedroom, Three Bathroom, Two Floors, and >= 2000 sqft

- Calculated the average price of a home for each year it was built that has 3 bedrooms, 3 bathrooms, two floors, and is greater than or equal to 2,000 square feet, rounded to two decimal places.

### 6. View Ratings for Average Price >= $350,000

- Calculated the "view" rating for the average price of a home, rounded to two decimal places, where the homes are greater than or equal to $350,000.
- Measured the runtime for this query.

### 7. Cache the Temporary Table

- Cached the temporary table `home_sales` for improved performance.

### 8. Check if the Table is Cached

- Checked if the `home_sales` temporary table is cached.

### 9. Query with Cached Data

- Ran a query on the cached data, filtering out view ratings with an average price greater than or equal to $350,000.
- Compared the runtime with the uncached version.

### 10. Partitioning the Data

- Partitioned the data by the "date_built" field and saved it in Parquet format.

### 11. Read Parquet Formatted Data

- Read the Parquet formatted data into a DataFrame.

### 12. Create Temporary Table for Parquet Data

- Created a temporary table (`temp_parquet`) for the Parquet data.

### 13. Query Parquet Data

- Ran a query on the Parquet data, filtering out view ratings with an average price greater than or equal to $350,000.
- Measured the runtime and compared it to the cached version.

### 14. Uncache Temporary Table

- Uncached the `home_sales` temporary table.

### 15. Check if the Table is Uncached

- Checked if the `home_sales` temporary table is no longer cached.


