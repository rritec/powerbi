Please listen below videos and read the material

[Intro to DW](https://youtu.be/NAuWUWmdmsE)

[OLTP Vs OLAP](https://youtu.be/KeJi1xDHQtA)

[Types of Schemas](https://youtu.be/XeMpv1Q3aJ8)


1. Name few business domains around you and understand how they collect data from customer.
    - Retail
        - amazon.in/amazon.com/amazon.co.uk        
    - Insurance
        - arbella
    - Healthcare
        - UHC
    - Banking
        - bankofamerica
    - IME
        - https://www.fox.com/
    - ... etc
2. What is data?
    - Any thing which helps to get some **meaningful information** is known as data.
    - Based on usage data Mainly two types
      -  Transactional Data
      -  Analytical Data
3. Transactional Data
    - Is run time data or day to day data
    - Is current and detail
    - Is useful to **Run** the business
    - Is stored in **OLTP**(On Line Transactional Processing)
    - Source of transactional data is mainly **web applications** and **mobile apps**
    - Example : ATM Transactions , Share market transactions..etc
    - ![image](https://user-images.githubusercontent.com/20516321/115664644-bb07c000-a35f-11eb-878a-ead2e05c2c1b.png)
4. Analytical Data
    - Is usuful to **ANALYSE**  the business
    - Is **Historical** and **Summarized**
    - Is stored in **OLAP**(On Line Analytical Processing) or **DW**(Data Warehouse )
    - Source of Analytical data is **OLTP**
5. Generic DW Flow or Architecture
    - ![image](https://user-images.githubusercontent.com/20516321/115807868-045f1a80-a407-11eb-9c80-458a606844d0.png)


6. DW Tools
    - ETL Tools
      - Informatica
      - Data Stage
      - Abintio
      - SSIS
      - ODI
      - OWB
      - BODI
    - Reporting or BI Tools
      - Power BI
      - Tableau
      - OBIEE
      - BI Publisher
      - Cognos
      - SAP-BO
      - DOMO
      - Qlick View
      - MicroStrategy 
7. OLTP Vs OLAP

    | OLTP      | OLAP(read only DB)(DSS)|
    | ----------- | ----------- |
    | Is useful to store Transactional data      | Is useful to store Analytical Data       |
    | Is useful to **run** the business   | Is useful to **analyze** the business        |
    | The nature of data is current and detail   | The nature of data is historical and summarized     |
    | OLTP Supports CRUD(Create ,Partially read,update,delete)   | OLAP supports only Read operations    |
    | It is a application oriented DB | It is a Subject oriented DB |
    | It is volatile | It is non Volatile |
    | No of users are more(customers+emp) | No of users are less (MM+HM) |
    | In OLTP we will use Normalized schema | In OLAP we will use denormalized schema |
8. Data Warehouse Definations
    - Different people have different definitions for a data warehouse.
    - The most popular definition came from Bill Inmon, who provided the following
        - A data warehouse is a subject-oriented, integrated, time-variant and non-volatile collection of data to support analysis.
        - Subject-Oriented: A data warehouse can be used to analyze a particular subject area. For example, "sales" can be a particular subject.
        - Integrated: A data warehouse integrates data from multiple data sources. For example, source A and source B may have different ways of identifying a product, but in a data warehouse, there will be only a single way of identifying a product.
        - Time-Variant: Historical data is kept in a data warehouse. For example, one can retrieve data from 3 months, 6 months, 12 months, or even older data from a data warehouse. This contrasts with a transactions system, where often only the most recent data is kept. For example, a transaction system may hold the most recent address of a customer, where a data warehouse can hold all addresses associated with a customer.
        - Non-volatile: Once data is in the data warehouse, it will not change. So, historical data in a data warehouse should never be altered.
    - Ralph Kimball provided a more concise definition of a data warehouse:
        - A data warehouse is a copy of transaction data specifically structured for query and analysis.
        - This is a functional view of a data warehouse. 
        - Kimball did not address how the data warehouse is built like Inmon did; rather he focused on the functionality of a data warehouse.
9. Tables
    - Dimension Tables (Keys + Descripitive Columns)
        - Role Play Dimensions
        - Slowly Changing Dimensions
            - SCD1
            - SCD2
            - SCD3
            - SCD4
            - SCD5
            - SCD6
        - Conformed Dimensions
        - Degenerated Dimension
        - Junk Dimension
    - Fact Tables (Keys + Mesure columns)

10. Schemas
    - A group of tables are called as schema 
        - Star 
        - Snow Flake
        - Constellation or mixed 
    - Star
        - Organizes data into a central fact table with surrounding dimension tables
        - Each dimension row has many associated fact rows
        - Dimension tables do not directly relate to each other
        - All Dimension Tables are de normalized
        - Optimized to read data
        - User friendly ,easy to understand
        - ![image](https://user-images.githubusercontent.com/20516321/115670440-0a9dba00-a367-11eb-9c39-abac453225f1.png)
    - Snow Flake
        - Normalized tables are used
        - Extended star schema
        - Two dimesiontables will be directly joined
        - Like star schema ,it  has only one fact table

    - Mixed Schema
        - Galaxy schema contains many fact tables with some common dimensions (conformed dimensions). 
        - This schema is a combination of many schemas
        - ![image](https://user-images.githubusercontent.com/20516321/115670843-7da73080-a367-11eb-8ed5-adac58cdffb0.png)
## Questions:
---
1. What type of attributes available in dimension?
    - Keys
    - Descriptive (example Product name,Product Size ..etc)
2. 1. What type of attributes available in Fact?
    - Keys
    - Measures (Revenue,Qty.. etc)
3. Based on usage the databases are divided into how many types?
    - OLTP > Runing the business
    - OLAP or DW > Analyzing the business
4. 












