# Sales Data Mart Project

This project involves creating a sales data mart using the AdventureWorks2019 database. The data mart is built using SQL Server Integration Services (SSIS) and SQL Server Analysis Services (SSAS) to provide a robust analysis and reporting solution.

## Project Overview

The goal of this project is to demonstrate the end-to-end process of building a sales data mart, from data extraction and transformation to building cubes for analysis.

### Key Components

- **Database Creation**: Set up the AdventureWorks2019 database as the source.
- **ETL Process**: Use SSIS to extract, transform, and load (ETL) data into the data mart.
  - **Dimension Tables**: Created using various SSIS components such as Lookup, Derived Column, and Merge Join.
  - **Fact Table**: Populated with sales data.
- **Analysis**: Use SSAS to create and deploy cubes for data analysis.

## Project Steps

### 1. Database Setup

1. Install and configure the AdventureWorks2019 database.
2. Create the necessary schema for the data mart.

### 2. ETL Process with SSIS

1. **Extract**: Pull data from AdventureWorks2019.
2. **Transform**:
   - Use **Lookup** transformations to retrieve related data.
   - Use **Derived Column** transformations to create new columns and perform data conversions.
   - Use **Merge Join** transformations to combine data from different sources.
3. **Load**: Insert the transformed data into dimension and fact tables in the data mart.

### 3. Data Mart Design

1. **Dimension Tables**:
   - Product Dimension  
   ![Product_DimTable](https://github.com/Kirolos107/SalesDataMart_SSIS_SSAS/assets/73123775/5b9aa412-3100-4f50-a87b-4b6878a7757f)  

   - Customer Dimension  
   ![Customer_DimTable](https://github.com/Kirolos107/SalesDataMart_SSIS_SSAS/assets/73123775/efd589a9-4e2f-4349-8413-8c5bc5fe3cf2)  

   - Territory Dimension  
   ![Territory_DimTable](https://github.com/Kirolos107/SalesDataMart_SSIS_SSAS/assets/73123775/5a05db58-34e9-482a-b639-764902c10767)  

   - Date Dimension  
   ![Date_DimTable](https://github.com/Kirolos107/SalesDataMart_SSIS_SSAS/assets/73123775/a60b9974-dca4-4b5f-8d5b-1f2fb70fe9a7)  

2. **Fact Table (Full & Incremental Load)**:  
   ![Sales_IncrementalLoad](https://github.com/Kirolos107/SalesDataMart_SSIS_SSAS/assets/73123775/2c20017b-ac2b-4d6c-a352-5a459fd4b90d)  
   ![Sales_FullLoad](https://github.com/Kirolos107/SalesDataMart_SSIS_SSAS/assets/73123775/cdd27691-f42f-46d9-8fbc-56ecc63d178f)  
   ![Sales_FactTable](https://github.com/Kirolos107/SalesDataMart_SSIS_SSAS/assets/73123775/0681ca09-54e0-46df-b2bc-a4134fb2eab9)  

### 4. Analysis with SSAS

1. Create a new SSAS project.
2. Define data sources and data source views.
3. Create cubes and define measures and dimensions.
4. Deploy the SSAS project and process the cubes.
5. Use SSAS tools to analyze the data.

## Tools and Technologies

- **SQL Server**: For database management and data storage.
- **SSIS**: For ETL processes.
- **SSAS**: For creating and analyzing cubes.
