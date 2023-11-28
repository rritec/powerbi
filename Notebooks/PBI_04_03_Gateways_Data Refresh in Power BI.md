
# Data Refresh
---

- How many types of sources are available?
  - On-Permise
    - excel
    - SqlServer
    - Oracle
    - ...etc 
  
  - Cloud
    - web
    - Azure SQL Database
    - snowflake    - 
    - ...etc
- For which type of sources required scheduling?
  - On-Permise
  - Scenerio:
      - Today 10 rows available in the Source(example: excel/sql server/oracle/teradata)(on - Permise Datasets)
      - you imported to PBI file
      - Developed reports
      - published report to power Bi service
      - After one month  5 more records added to excel and 2 records of excel updated and 1 record of excel deleted.Now total number of records in excel is 14
      - However if i go and run report in **power Bi service** ,iam seeing old data (10 rows). How to fix it?
      - 
 
2. Power BI Service(Azure Cloud) Communicates On -Permise Datasets by using ............?
  - Gateway
## What is an on-premises data gateway?
- The on-premises data gateway acts as a bridge to provide quick and secure data transfer between on-premises data (data that isn't in the cloud) and several Microsoft cloud services.
- These cloud services include Power BI, PowerApps, Power Automate, Azure Analysis Services, and Azure Logic Apps.
- By using a gateway, organizations can keep databases and other data sources on their on-premises networks, yet securely use that on-premises data in cloud services.

![image](https://user-images.githubusercontent.com/20516321/113988805-74996800-986d-11eb-888f-c7255a071f55.png)

## Types of gateways
- There are two different types of gateways, each for a different scenario:

  1. **On-premises data gateway** allows multiple users to connect to multiple on-premises data sources. You can use an on-premises data gateway with all supported services, with a single gateway installation. This gateway is well-suited to complex scenarios with multiple people accessing multiple data sources.It is also called as **Enterprise** or **Standalone** Gateway

  2. **On-premises data gateway (personal mode)** allows one user to connect to sources, and can’t be shared with others. An on-premises data gateway (personal mode) can be used only with Power BI. This gateway is well-suited to scenarios where you’re the only person who creates reports, and you don't need to share any data sources with others.

## Download and install a personal mode gateway

  1. [Download the personal mode gateway.](https://go.microsoft.com/fwlink/?LinkId=2116848&clcid=0x409)
  2. In the gateway installer, enter the default installation path, accept the terms of use, and then select Install.

      ![image](https://user-images.githubusercontent.com/20516321/113989982-9d6e2d00-986e-11eb-9961-a3fa02477f21.png)

  3. Enter the email address for your Office 365 organization account, and then select Sign in.
    ![image](https://user-images.githubusercontent.com/20516321/113990054-b1b22a00-986e-11eb-8788-eeb89b005a05.png)

  4. You're now signed in to your account. Select Close.
      ![image](https://user-images.githubusercontent.com/20516321/113990114-c393cd00-986e-11eb-9ac1-ca3a6016a1ed.png)
 ## Schedule Dataset developed using Excel/SQL Server Source

  1. Follow regular process and develop a report from excel source
  2. Publish it
  3. In Power BI Service > click on dataset schedule and set credentials and time accordingly
  4. 
## Incremental Refresh

  1. Open Power BI Desktop
  2. Import DimDate, DimCustomer, FactInternetSales from Sql Server AdventureWorksDW2012 database
  3. Develop a table visulization, by dragging **orderdate** column from **FactInternetSales** > Set **Orderdate** as **date** column  > set aggregation rule as **earliest** . Again drag **orderdate** column from **FactInternetSales** table > set **orderdate** as date column > set aggregation rule as **latest** date
  ![image](https://user-images.githubusercontent.com/20516321/129829244-0af234a9-016d-4e5e-a4c1-6280c9c6cef5.png)
  4. In **PowerQueryEditor** window create two parameters with the name of **RangeStart** and **RangeEnd** and set below values.
  
  ![image](https://user-images.githubusercontent.com/20516321/129829544-1900ae16-10b0-4801-8faa-e35975a94ca9.png)


  4. Apply custom filter on **FactInternetSales > Orderdate** column by using above parameters(RangeStart/RangeEnd)
  5. close and apply
  6. In power View > right click on FactInternetsales>click on Incremental Refresh select required options.

## Home WOrk

[Create Power automate flow to refresh PowerBI Dataset](https://github.com/rritec/PowerAutomate/blob/main/Create%20Power%20automate%20flow%20to%20refresh%20PowerBI%20Dataset.md)


Reference: 
- https://docs.microsoft.com/en-us/data-integration/gateway/service-gateway-install
- https://docs.microsoft.com/en-us/power-bi/connect-data/refresh-data
- https://docs.microsoft.com/en-us/power-bi/admin/service-premium-incremental-refresh

## Questions
----
1. With **Pro** Licence, how many times we can schedule/Refresh the dataset in a given day?
  - **8** Times
2. With **Premium** Licence, how many times we can schedule/Refresh the dataset in a given day?
  - **48** Times
3. In Incrmental Refresh what are the parameters are manadatory?
  - RangeStart
  - RangeEnd
4. In Incrmental refresh what is the importance of **Detect data changes**
  - [Refer](https://docs.microsoft.com/en-us/power-bi/connect-data/incremental-refresh-overview#4---detect-data-changes)
5. In Incrmental refresh what is the importance of **Only Refresh Complete Days**
  - [Refer](https://docs.microsoft.com/en-us/power-bi/connect-data/incremental-refresh-overview#5---only-refresh-complete-days)
6. What is Query Folding?
  -  Incremental refresh is designed for data sources that support query folding, which is Power Query's ability to generate a single query expression to retrieve and transform source data. Most data sources that support SQL queries support query folding. Data sources like flat files, blobs, and some web feeds often do not.
7. Incremental Refresh, can you apply on **Excel** Data source?
  - No


