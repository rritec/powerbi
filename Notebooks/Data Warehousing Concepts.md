1. Name few business domains around you and understand how they collect data from customer.
    - Retail
    - Insurance
    - Healthcare
    - Banking
    - ... etc
2. What is data?
    - Any thing which helps to get some meaningful information is known as data.
    - Based on usage data Mainly two types
      -  Transactional Data
      -  Analytical Data
3. Transactional Data
    - Is run time data or day to day data
    - Is current and detail
    - Is useful to Run the business
    - Is stored in OLTP(On Line Transactional Processing)
    - Source of transactional data is mainly web applications and mobile apps
    - Example : ATM Transactions , Share market transactions..etc
    - ![image](https://user-images.githubusercontent.com/20516321/115664644-bb07c000-a35f-11eb-878a-ead2e05c2c1b.png)
4. Analytical Data
    - Is usuful to ANALYSE  the business
    - Is Historical and summarized 
    - Is stored in OLAP(On Line Analytical Processing) or DW(Data Warehouse )
    - Source of Analytical data is OLTP
5. Generic DW Flow or Architecture
    - ![image](https://user-images.githubusercontent.com/20516321/115664889-19cd3980-a360-11eb-803d-ecf61a778c20.png)

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







8. 








