# Velocipede Vista: Crafting Insights from Global Cycling Data


# AdventureWorks Data Warehouse Project

## Overview

The project focuses on creating a data warehouse for AdventureWorks, a company in the bicycle sales industry, aiming to centralize and consolidate data for advanced analytics.


## Objectives

- Consolidate data from various sources for better reporting and analytics.
- Optimize data utilization for insightful analysis.

## 💾 Dataset

**AdventureWorks** is a database provided by Microsoft for free on online platforms. It is a product sample database originally published by Microsoft to demonstrate the supposed design of a SQL server database using SQL server 2008. Here are some key points to know about AdventureWorks:
- AdventureWorks database supports a manufacturing MNC named Adventure Works Cycles.
- It is a sample Online Transaction Processing (or OLTP) database, which is a type of data processing where multiple transactions occur concurrently. These are shipped by Microsoft with all of their SQL server products.

> For this project I used the **Lightweight (LT) data**: a lightweight and pared down version of the OLTP sample. [Download here](https://learn.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver16&tabs=ssms)

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

### Dim Dataflow
![all_dim](https://github.com/Famz21/DWH/assets/125658739/9fdfabaf-0ed0-41cd-9e7f-de2d226b5cde)


### DimDate Dataflow
![DimDate](https://github.com/Famz21/DWH/assets/125658739/88003331-1a00-4a29-abd8-46e6f6432d54)


### DimCurrency Dataflow
![Currency](https://github.com/Famz21/DWH/assets/125658739/abcc6b44-fc28-4951-8bb9-ffea68a78a06)

### DimCustomer Dataflow
![customerView](https://github.com/Famz21/DWH/assets/125658739/8baf417e-57d5-426a-b64f-8829f5b94751)


### DimStore Dataflow
![dimstore](https://github.com/Famz21/DWH/assets/125658739/dea39f5f-e092-4d60-b730-540717e52146)


### DimPromotion Dataflow
![promotion](https://github.com/Famz21/DWH/assets/125658739/1ee5ebae-32e4-4324-87ac-f457e9774f24)


### DimSalesTerritory Dataflow
![sales_ter](https://github.com/Famz21/DWH/assets/125658739/7996a3ec-3f63-4c37-acc2-abf658f58c1f)


### DimGeography Dataflow
![geo_view](https://github.com/Famz21/DWH/assets/125658739/44178ecb-5ceb-4c07-be74-4b4a7daf3b6a)





## Tools and Technologies

- SQL Server Management Studio (SSMS)
- ODBC Drivers
- ETL Tools

## Conclusion

This project enables AdventureWorks to leverage data for strategic decisions, covering the journey from data source identification to deployment in a production environment.

