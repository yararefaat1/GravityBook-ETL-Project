# GravityBook-ETL-Project
It involves the design and implementation of an ETL process using (SSIS) and (SSMS).. Key features include the creation of surrogate keys, enforcement of foreign key constraints, and the development of Date_Dim and Time_Dim tables to maintain referential integrity. 

Your README file provides a solid outline of the steps involved in your ETL process using SSIS and SSMS. However, it could benefit from some adjustments for clarity, professionalism, and structure. Here’s a revised version:

ETL Process Using SSIS and SSMS
This project outlines the steps taken to design and implement a robust ETL (Extract, Transform, Load) process using SQL Server Integration Services (SSIS) and SQL Server Management Studio (SSMS). The goal was to ensure accurate data integration, consistency, and integrity across the data warehouse.

# Steps Involved
## Connection Verification

- Verified connections between the Source and Destination in each ETL cycle to prevent incorrect data loading.
Column Mapping and SQL Query Optimization

- Ensured accurate column mapping to maintain data consistency and integrity.
- Used SQL commands, particularly "Left Outer Join," to minimize duplicates and ensure that all necessary records were captured.
Data Deduplication and Source Integration

- Removed duplicates using the "Sort" function by enabling the "Remove rows with duplicate sort values" option.
- Integrated multiple data sources using "Union ALL," ensuring consistent column structures across sources.

## Dimension Table Setup in SSMS

- Created surrogate keys for each dimension and set them as primary keys to uniquely identify records.
- Applied unique constraints to maintain the uniqueness of business keys after removing the primary key constraints.
- Developed Date_Dim and Time_Dim tables for time-related dimensions.
- Defined foreign key constraints in the fact table to reference Date_Dim and Time_Dim, ensuring referential integrity.
- Fact Table Loading in SSIS

- Extracted timeSK and DateSK from the dimension tables and loaded them into the fact table to maintain proper relationships.
  
