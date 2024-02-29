# DWH

## 📝 Table of Contents
1. [Project Overview](#introduction)
2. [Key Insights](#key-insights)
3. [Project Architecture](#project-architecture)  
  3.1. [Data Ingestion](#data-ingestion)  
  3.2. [Data Transformation](#data-transformation)  
  3.3. [Data Loading](#data-loading)  
  3.4. [Data Reporting](#data-reporting)
4. [Credits](#credits)
5. [Contact](#contact)

<a name="introduction"></a>
## 🔬 Project Overview 

This an end-to-end data engineering project on the Azure cloud. Where I did data ingestion from a on-premise SQL Server to Azure Data Lake using Data Factory to transformation using Databricks and Spark, loading to Synapse, and reporting using PowerBI. Also, I used Azure Active Directory (AAD) and Azure Key Vault for the data monitoring and governance purpose. 

### 💾 Dataset

**AdventureWorks** is a database provided by Microsoft for free on online platforms. It is a product sample database originally published by Microsoft to demonstrate the supposed design of a SQL server database using SQL server 2008. Here are some key points to know about AdventureWorks:
- AdventureWorks database supports a manufacturing MNC named Adventure Works Cycles.
- It is a sample Online Transaction Processing (or OLTP) database, which is a type of data processing where multiple transactions occur concurrently. These are shipped by Microsoft with all of their SQL server products.

> For this project I used the **Lightweight (LT) data**: a lightweight and pared down version of the OLTP sample. [Download here](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms)


# AdventureWorks Data Warehouse Project

## Overview

The project focuses on creating a data warehouse for AdventureWorks, a company in the bicycle sales industry, aiming to centralize and consolidate data for advanced analytics.

## Objectives

- Consolidate data from various sources for better reporting and analytics.
- Optimize data utilization for insightful analysis.

## Phases

1. **Define Requirements**: Understanding business goals, identifying data sources, and defining data granularity and architecture.
2. **ETL Workflow**: Steps for extracting, transforming, and loading data into the DW.
3. **Testing and Deployment**: Includes unit testing, integration testing, and deployment to production.

## Architecture

Adopts a star schema design for optimized query performance and simplicity.

![schema](https://github.com/Famz21/DWH/assets/125658739/2a37956b-1324-4a2e-bf2f-a42f06013164)

## ETL Process

By using SSIS, I perform ETL process involves extracting data from Csv files, transforming it to fit our data warehouse schema, and loading it,also i have implemented incremental loading and SCD types to efficiently manage data updates.

### FactStoreSales Dataflow
![store_sales](https://github.com/Famz21/DWH/assets/125658739/dcee85c6-f321-4c7a-81dd-00a81864eb2f)

### FactOnlineSales Dataflow
![sales2](https://github.com/Famz21/DWH/assets/125658739/c2079a20-5882-44fa-9c1f-762e3f086ee2)

### DimDate Dataflow




## Tools and Technologies

- SQL Server Management Studio (SSMS)
- ODBC Drivers
- ETL Tools

## Conclusion

This project enables AdventureWorks to leverage data for strategic decisions, covering the journey from data source identification to deployment in a production environment.

