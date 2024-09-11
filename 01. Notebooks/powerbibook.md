.



![image](https://user-images.githubusercontent.com/20516321/219373758-0487c4a9-1a42-4402-a849-41398b3d3c77.png)

# Whatsapp: 8374 899 166
# Online/Class Room Training

.


.


.


.
.















# Power BI
1. **[Data Warehousing Concepts](#Data-Warehousing-Concepts)**<br>
2. **[Introduction Installation](#Introduction-Installation)**<br>
3. **[Power Query Editor Shape data using Excel as source](#Power-Query-Editor-Shape-data-using-Excel-as-source)**<br>
4. **[Power Query Editor Shape data using MySql as input](#Power-Query-Editor-Shape-data-using-MySql-as-input)**<br>
5. **[Power Query Editor Shape data using SQL Server as input](#Power-Query-Editor-Shape-data-using-SQL-Server-as-input)**<br>
6. **[Optional](#Optional)**<br>
7. **[M-Language](#M-Language)**<br>
8. **[Power Query Editor Combine Data](#Power-Query-Editor-Combine-Data)**<br>
9. **[Project1 Power Query Editor Lab](#Project1-Power-Query-Editor-Lab)**<br>
10. **[Power Query Editor Knowledge Test](#Power-Query-Editor-Knowledge-Test)**<br>
11. **[Power Pivot Modeling Part1](#Power-Pivot-Modeling-Part1)**<br>
12. **[Power Pivot Modeling Part2](#Power-Pivot-Modeling-Part2)**<br>
13. **[Power Pivot DAX Metrics](#Power-Pivot-DAX-Metrics)**<br>
14. **[DAX iterator Functions](#DAX-iterator-Functions)**<br>
15. **[DAX Studio](#DAX-Studio)**<br>
16. **[Recap](#Recap)**<br>
17. **[Power Pivot Modeling Lab](#Power-Pivot-Modeling-Lab)**<br>
18. **[Exam](#Exam)**<br>
19. **[Power View Visualization Lab](#Power-View-Visualization-Lab)**<br>
20. **[Power View Hierarchy Drill down drill up](#Power-View-Hierarchy-Drill-down-drill-up)**<br>
21. **[Power View Drill Through](#Power-View-Drill-Through)**<br>
22. **[Types of Filter](#Types-of-Filter)**<br>
23. **[Groups Bins](#Groups-Bins)**<br>
24. **[Conditional Formatting](#Conditional-Formatting)**<br>
25. **[Power BI Service](#Power-BI-Service)**<br>
26. **[Create Apps](#Create-Apps)**<br>
27. **[Parameters](#Parameters)**<br>
28. **[Gateways Data Refresh in Power BI](#Gateways-Data-Refresh-in-Power-BI)**<br>
29. **[Deployment Pipelines](#Deployment_Pipelines)**<br>
30. **[Bookmarks Actions Buttons Images](#Bookmarks-Actions-Buttons-Images)**<br>
31. **[Power BI Import Vs Direct Query Vs Live Connection](#Power-BI-Import-Vs-Direct-Query-Vs-Live-Connection)**<br>
32. **[Run Python scripts in Power BI Desktop](#Run-Python-scripts-in-Power-BI-Desktop)**<br>
33. **[SSAS Multidimensional Models in PowerBI Desktop](#SSAS-Multidimensional-Models-in-PowerBI-Desktop)**<br>
34. **[Connect to a Snowflake computing warehouse in Power BI Desktop](#Connect-to-a-Snowflake-computing-warehouse-in-Power-BI-Desktop)**<br>
35. **[row level security (RLS)](#row-level-security-(RLS))**<br>
36. **[Power BI Cmdlets for Windows PowerShell and PowerShell Core](#Power-BI-Cmdlets-for-Windows-PowerShell-and-PowerShell-Core)**<br>
37. **[Paginated Reports](#Paginated-Reports)**<br>
38. **[SSRS](#SSRS)**<br>
39. **[Migrate SSRS to PowerBI](#Migrate-SSRS-to-PowerBI)**<br>
40. **[Power BI Interview Questions](#Power-BI-Interview-Questions)**<br>


#  Data Warehousing Concepts

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



# Introduction Installation
---

##  What is BI ?
---
1. BI(Business Intelligence) is a processes that convert **Raw Data** into **Meaningful Information**
1. The **meaningful information** drives **profitable business actions**

## Do you know any BI tools?
---
1. Power BI
1. Tableau
1. Cognos
1. Bo
1. OBIEE
1. Domo
1. Qlick View/Sense
... etc

### Out of these all BI tools, which is best? why ?
---
- According to world's leading research and advisory company **Power BI** is best. 
    - [Gartner Report](https://powerbi.microsoft.com/en-us/blog/microsoft-named-a-leader-in-gartners-2020-magic-quadrant-for-analytics-and-bi-platforms/)
    - [Forrester Report](https://info.microsoft.com/ww-landing-Forrester-Wave-Enterprise-BI-platforms-website.html?LCID=EN-US)


    

## What is Power BI?
---
1. Power BI is a business analytics solution that lets you visualize your data and share **insights** across your organization, or embed them in your app or website.
1. Connect to **hundreds of data sources** and bring your data to **life** with **live dashboards** and **reports**.
1. [Visit for more information](https://powerbi.microsoft.com/en-us/what-is-power-bi/)

## Why Power BI?
---
1. Create data dashboards and visualizations in **minutes**
1. Put BI in everyone’s hands—**economically**. Please see the price of Tableau and Power BI    
    - [Power BI Price](https://powerbi.microsoft.com/en-us/pricing/)
    - [Tableau Price](https://www.tableau.com/pricing/teams-orgs#online)
1. Unify **self-service** and enterprise analytics
1. Accelerate big data prep with **Azure**
1. Find answers fast with industry-leading **AI**
1. Get unparalleled **Excel** integration
1. Turn **insights** into **action**
1. **Stream analytics** in **real time**
1. [Visit for more information](https://powerbi.microsoft.com/en-us/why-power-bi/)

## Do you know Power BI products?
---
1. **Power BI Desktop**(Windows based software)
    - Create rich,interactive reports with visual analytics at your fingertips
    - Go from `data` →  `insight` →  `action` with Power BI Desktop
    - Connect to your data, wherever it is
    - Prep and model your data with ease
    - Provide advanced analytics with the familiarity of Excel
    - Create interactive reports customized for your business
    - Power BI Desktop is nothing but three tools of excel 
        - Power Query or Power Query Editor
        - Power Pivot
        - Power View
            - [Read More](https://support.office.com/en-us/article/power-query-overview-and-learning-ed614c81-4b00-4291-bd3a-55d80767f81d)
            
2. **Power BI Service**(MSFT Cloud)
    - Dashboards are developed here
    - Conduct data-driven collaboration
    - Discover insights quickly
    - Get more done with familiar tools
    - Govern your data securely
3. Power BI Mobile
4. Power BI Embedded
5. Power BI Report Server
        

# Install Power BI Desktop
---
- Download software [here](https://www.microsoft.com/en-us/download/details.aspx?id=58494)
- Run the MSI installer and follow the setup steps    

![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation9.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation8.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation7.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation6.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation5.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation4.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation3.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation2.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation1.png?raw=true)
[Reference](https://docs.microsoft.com/en-us/power-bi/desktop-get-the-desktop)

# MSFT SQL Server Installation
---

## Install MSFT SQL Server Database
---

1. Download Sqlserver Developer edition [here](https://www.microsoft.com/en-au/sql-server/sql-server-downloads)

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0132.png?raw=true)
    
1. Run below **.exe** file

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0126.png?raw=true)
1. Click on **Basic**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0127.png?raw=true)
1. Click on **Accept**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0128.png?raw=true)
1. Click on **Install**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0130.png?raw=true)
1. Observe connections info

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0129.png?raw=true)  
   

    

## Instal SQL Server Management Studio (SSMS) 
---

1. Download SQL Server Management Studio [here](https://www.microsoft.com/en-au/sql-server/sql-server-downloads)
1. Double Click on exe file

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0133.png?raw=true)
1.   Click on **Install**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0134.png?raw=true)
1.   Click on **Restart**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0136.png?raw=true)   


## Restore sample data
---

1. Follow below link download and restore sample data **AdventureWorksDW2012.bak**
https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15

## Instal MSBI (Download SQL Server Data Tools (SSDT))
---

1. Download Sqlserver Developer edition https://www.microsoft.com/en-au/sql-server/sql-server-downloads

direct link : https://docs.microsoft.com/en-us/sql/ssdt/download-sql-server-data-tools-ssdt?view=sql-server-ver15#ssdt-for-vs-2017-standalone-installer

1. Double Click on exe file

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0136.png?raw=true)
1.   Click on **install**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0137.png?raw=true)
1.   Click on **install**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0138.png?raw=true)   


# MySql Installation(Optional)
---
1. Download the software 
    https://dev.mysql.com/downloads/file/?id=508936
3. Ckick in msi file and install it
![image](https://user-images.githubusercontent.com/20516321/148321034-5bbd5b60-57e6-42c4-ae60-3fb446f6c1b1.png)

4. Click on Next
![image](https://user-images.githubusercontent.com/20516321/148321192-cef7b0f0-d38a-417e-b0a4-3827711da9e3.png)

5. Observe all components
![image](https://user-images.githubusercontent.com/20516321/148321246-8f013719-ee9a-428a-844b-7134cc97aaf0.png)
6. Click on Next
    ![image](https://user-images.githubusercontent.com/20516321/148321730-ebf433d9-08cb-4b66-985e-98d27a9be83b.png)

7. Provide **root** user password and notedown some where
    ![image](https://user-images.githubusercontent.com/20516321/148321849-dff93321-3f00-466c-b3ca-af97b5758a5f.png)




## Interview Questions
-----
1. What are the **key components** of power BI.
    1. Power BI Desktop(Power Query/Power Pivot/Power View)
    2. Power BI Service
    3. Power BI Mobile
    4. Power BI Maps
    5. Power BI Embeded Analytics
    
# Power Query Editor Shape data using Excel as source
    - It has mainly three Components
        - Power Query Editor(Extract + Transforming + Loading into PBIX file)
        - Power Pivot (Model + DAX)
        - Power View or Report View
# Power Query Editor
- It is also known as `Power Query`
# Download all materials and data
1. Download materials [here](https://github.com/rritec/powerbi/archive/refs/heads/master.zip)
1. Create one folder on desktop with the name of **PowerBI_work**
1. Move above **powerbi-master.zip** file to **PowerBI_work** folder
1. Right click on **powerbi-master.zip** file > Click on **Extract All**
1. Observe all materials and Labs


## Import scott data from excel

![image](https://user-images.githubusercontent.com/20516321/196328872-9932cfa7-18cb-4b14-b609-e87f4d12bda2.png)


1. Go to windows search > type **Power BI** > Open **Power BI Desktop** > Click on **Get Data** > Click on **File** > Click on **Excel**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0081.png?raw=true)
    
1. Click on **Connect** > Select **Labdata/Lab1/scottdata.xlsx** > Click on **open**
1. In **Navigator** select all three tables > Click on **Transform Data**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0082.png?raw=true)

## Power Query has `5` main parts
1. Menu Bar(Home/Transform/Add Column/View/Tools/Help)
1. Queries Pane
1. Query Settings Pane
1. Work area
1. Formula Bar

## Replace in `emp` table `comm` column `null` with `0`
1. In **Queries** pane  > Select **emp** table > select **comm** column
1. In the **toolbar** > Click on **Replace Values** > type as shown in below image
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0083.png?raw=true)



## Rename column name `ename` as `Employee Name`
1. In **Queries** pane > select **emp** > Right click on **ename** column 

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0087.png?raw=true)
    
1. Click on **rename** and name it as **Employee Name** > press enter

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0088.png?raw=true)
    
## Create `totalsal` column
1. In the **Menu bar** > Click on **Add Column** > Click on **Custom Column** > Name it as **totalsal**
1. Develop formula as shown in below image > Click on **ok**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0084.png?raw=true)
1. Observe output
   
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0086.png?raw=true)




## Observe Data Types
1. Decimal Number
2. Fixed Decimal Number
3. Whole Number
4. Percentage
5. Date/Time
6. Date
7. Time
8. Date/Time/Timezone
9. Duration
10. Text
11. True/False
12. Binary
## Change data type of TotalSal to decimal numbar
1. Right click on **totalsal** column > click on **Change type** > Click on **Decimal Number**

## AutoFilter/Basic Filter
### Filter `sal` column to display only greater than `900`
1. Click on **sal** column down arrow mark > Click on **Number Filters** > Click on **Greater Than** > type **900** > Click on **ok**

## Save the report
1. Go to **File** menu > click on **save** > Select **powerbi_work** folder > name it as **PBI_01_02_Power Query Editor Shape data using Excel as source** > click on **ok**


## Publish the report

1. Open https://app.powerbi.com/
1. Signin with username and password given to you by your instructor
2. In the left Navigation Pane > Click on Workspaces > Click on Create a Workspace > provide workspace name as rritec - workspace > click on Save
3. In **Power BI Desktop** > click on **signin** and pass username and password
4. Click on **publish** > Select above workspace **rritec - workspace** > click on ok
5. Go to **power BI service** > observe report
    

## Reference 

https://docs.microsoft.com/en-us/power-bi/fundamentals/desktop-getting-started

https://docs.microsoft.com/en-us/power-bi/connect-data/desktop-shape-and-combine-data

https://docs.microsoft.com/en-us/power-bi/transform-model/desktop-common-query-tasks

https://docs.microsoft.com/en-us/power-bi/desktop-add-custom-column

https://docs.microsoft.com/en-us/powerquery-m/power-query-m-function-reference


```python

```
## Questions
1. **Power BI** Key Components?
    - Power BI Desktop
    - Power BI Service
    - Power BI Mobile
1. **Power BI Desktop** Key components
    - Power Query Editor
    - Power Pivot
    - Power View
1. Power Query Editor useing which language?
    - M - Language
1. Can we import 2 sheets from excel workbook which has 5 sheets?
    - Yes
1. Each Sheet is called as what in power Query Editor?
    - Query
1. Can we reorder Transformation steps in **Qurry Settings**?
    - Yes
1. What is the extension of Power BI File?
    - .PBIX
1. The calculation in Power Query Editor is called as ?
    - Co**M**uting Column
1. Can you name some of the Power BI supporting Data Types?
    - Whole Number
    - Deciambal
    - Text
    - Date
    - True/False(Bool)
    - DateTime
    - .... etc
    
1. In how many ways we can see the list of query applied steps?
   - Query setting pane
   - Advance Editor
1. In Excel how many kinds of data containers available?
    - Sheet
    - Table
1. How Many Data Sources/Data bases worked ?
    - Flat Files(Excel,Csv,Tab delimited,Json,XML...etc)
    - Relational Databases (MS Sql Server,Oracle,Teradata,MySql,BigData Hive,...etc)
    - Cloud Databases(Snow Flake,Azure SQl Database,Azure Synapse,Azure Blobs...etc)


# Power Query Editor Shape data using MySql as input

![image](https://user-images.githubusercontent.com/20516321/196849404-a9371f5d-6a66-4d5c-9285-75e3131c8332.png)


1. MySql is a oracle product
1. Install **MySql** software by following [this link](https://github.com/rritec/powerbi/blob/master/Notebooks/PBI_01_01_Introduction_Installation.md#mysql-installationoptional)
1. Open **MySql Workbench** > if required create **new connection** or use **existing connection** > Click on **New SQL Tab for execution of queries**
1. In **Navigator** Window in empty space > Right Click > click on **Create Schema** > Provide schema name as **rritecdb** > click on **apply** > click on **apply** > Click on **Finish**

**or**

run below script 

``` sql
CREATE SCHEMA rritecDB;
```
``` sql
USE rritecdb;
```

## Load Data
``` sql
drop table if exists emp;

drop table if exists dept;

drop table if exists salgrade;

drop table if exists emp10;

drop table if exists emp20;

drop table if exists emp30;
```

``` sql
CREATE TABLE `emp` (
  `empno` decimal(4,0) NOT NULL,
  `ename` varchar(10) DEFAULT NULL,
  `job` varchar(9) DEFAULT NULL,
  `mgr` decimal(4,0) DEFAULT NULL,
  `hiredate` date DEFAULT NULL,
  `sal` decimal(7,2) DEFAULT NULL,
  `comm` decimal(7,2) DEFAULT NULL,
  `deptno` decimal(2,0) DEFAULT NULL,
  `test` varchar(100) DEFAULT NULL
) ;


INSERT INTO emp (empno,ename,job,mgr,hiredate,sal,comm,deptno,test) VALUES 
(7369,'SMITH','CLERK',7902,'1980-12-17',800.00,NULL,20,'1')
,(7499,'ALLEN','SALESMAN',7698,'1981-02-20',1600.00,300.00,30,'1')
,(7521,'WARD','SALESMAN',7698,'1981-02-22',1250.00,500.00,30,'1')
,(7566,'JONES','MANAGER',7839,'1981-04-02',2975.00,NULL,20,'1')
,(7654,'MARTIN','SALESMAN',7698,'1981-09-28',1250.00,1400.00,30,'1')
,(7698,'BLAKE','MANAGER',7839,'1981-05-01',2850.00,NULL,30,'1')
,(7782,'CLARK','MANAGER',7839,'1981-06-09',2450.00,NULL,10,'1')
,(7788,'SCOTT','ANALYST',7566,'1982-12-09',3000.00,NULL,20,'1')
,(7839,'KING','PRESIDENT',NULL,'1981-11-17',5000.00,NULL,10,'1')
,(7844,'TURNER','SALESMAN',7698,'1981-09-08',1500.00,0.00,30,'1')
,(7876,'ADAMS','CLERK',7788,'1983-01-12',1100.00,NULL,20,'1')
,(7900,'JAMES','CLERK',7698,'1981-12-03',950.00,NULL,30,'1')
,(7902,'FORD','ANALYST',7566,'1981-12-03',3000.00,NULL,20,'1')
,(7934,'MILLER','CLERK',7782,'1982-01-23',1300.00,NULL,10,'1')
,(1234,'RamReddy','DS',7839,'1981-12-03',2400.00,100.00,50,'1')
;

CREATE TABLE `dept` (
  `deptno` decimal(2,0) DEFAULT NULL,
  `dname` varchar(14) DEFAULT NULL,
  `loc` varchar(13) DEFAULT NULL,
  `test` varchar(100) DEFAULT NULL
) ;

INSERT INTO dept (deptno,dname,loc,test) VALUES 
(10,'ACCOUNTING','NEW YORK','1')
,(20,'RESEARCH','DALLAS','1')
,(30,'SALES','CHICAGO','1')
,(40,'OPERATIONS','BOSTON','1')
;

CREATE TABLE salgrade(
  grade decimal(1),
  losal decimal(4),
  hisal decimal(4)
);

INSERT INTO salgrade VALUES 
(1, 700, 1200)
,(2, 1201, 1400)
,(3, 1401, 2000)
,(4, 2001, 3000)
,(5, 3001, 9999);

CREATE TABLE `emp10` (
  `empno` decimal(4,0) NOT NULL,
  `ename` varchar(10) DEFAULT NULL,
  `job` varchar(9) DEFAULT NULL,
  `mgr` decimal(4,0) DEFAULT NULL,
  `hiredate` date DEFAULT NULL,
  `sal` decimal(7,2) DEFAULT NULL,
  `comm` decimal(7,2) DEFAULT NULL,
  `deptno` decimal(2,0) DEFAULT NULL,
  `test` varchar(100) DEFAULT NULL
) ;


INSERT INTO emp10 (empno,ename,job,mgr,hiredate,sal,comm,deptno,test) VALUES 
(7782,'CLARK','MANAGER',7839,'1981-06-09',2450.00,NULL,10,'1')
,(7839,'KING','PRESIDENT',NULL,'1981-11-17',5000.00,NULL,10,'1')
,(7934,'MILLER','CLERK',7782,'1982-01-23',1300.00,NULL,10,'1')
;

CREATE TABLE `emp20` (
  `empno` decimal(4,0) NOT NULL,
  `ename` varchar(10) DEFAULT NULL,
  `job` varchar(9) DEFAULT NULL,
  `mgr` decimal(4,0) DEFAULT NULL,
  `hiredate` date DEFAULT NULL,
  `sal` decimal(7,2) DEFAULT NULL,
  `comm` decimal(7,2) DEFAULT NULL,
  `deptno` decimal(2,0) DEFAULT NULL,
  `test` varchar(100) DEFAULT NULL
) ;


INSERT INTO emp20 (empno,ename,job,mgr,hiredate,sal,comm,deptno,test) VALUES 
(7369,'SMITH','CLERK',7902,'1980-12-17',800.00,NULL,20,'1')
,(7566,'JONES','MANAGER',7839,'1981-04-02',2975.00,NULL,20,'1')
,(7788,'SCOTT','ANALYST',7566,'1982-12-09',3000.00,NULL,20,'1')
,(7876,'ADAMS','CLERK',7788,'1983-01-12',1100.00,NULL,20,'1')
,(7902,'FORD','ANALYST',7566,'1981-12-03',3000.00,NULL,20,'1')
;

CREATE TABLE `emp30` (
  `empno` decimal(4,0) NOT NULL,
  `ename` varchar(10) DEFAULT NULL,
  `job` varchar(9) DEFAULT NULL,
  `mgr` decimal(4,0) DEFAULT NULL,
  `hiredate` date DEFAULT NULL,
  `sal` decimal(7,2) DEFAULT NULL,
  `comm` decimal(7,2) DEFAULT NULL,
  `deptno` decimal(2,0) DEFAULT NULL,
  `test` varchar(100) DEFAULT NULL
) ;


INSERT INTO emp30 (empno,ename,job,mgr,hiredate,sal,comm,deptno,test) VALUES 
(7499,'ALLEN','SALESMAN',7698,'1981-02-20',1600.00,300.00,30,'1')
,(7521,'WARD','SALESMAN',7698,'1981-02-22',1250.00,500.00,30,'1')
,(7654,'MARTIN','SALESMAN',7698,'1981-09-28',1250.00,1400.00,30,'1')
,(7698,'BLAKE','MANAGER',7839,'1981-05-01',2850.00,NULL,30,'1')
,(7844,'TURNER','SALESMAN',7698,'1981-09-08',1500.00,0.00,30,'1')
,(7900,'JAMES','CLERK',7698,'1981-12-03',950.00,NULL,30,'1')
;
```
## Import below tables into Power BI

1. emp
1. dept
1. salgrade
1. emp10
1. emp20
1. emp30


1. Open **Power BI Desktop** > Click on **Get Data** > Click on **Databases** > select **MySql Database** > click on **connect**

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0089.png?raw=true)
 
1. provider server as **localhost** > Database as **rritec** > Click on **ok**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0090.png?raw=true)
    
1. Select all the tables as shown below > clcik on **LoadData** 

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0091.png?raw=true)


## Do all exercise of Previous chapter [PBI_01_02_Power Query Editor Shape data using Excel as source](https://github.com/rritec/powerbi/blob/master/Notebooks/PBI_01_02_Power%20Query%20Editor%20Shape%20data%20using%20Excel%20as%20source.md)

## Questions
1. What is the official tool, to query MySql database?
    - MySQL Workbench
2. 
```python

```
# Power Query Editor Shape data using SQL Server as input
---
**Note:** Mostly as **BI** developer, we wont get chance to create databases,tables and loading data. In our training program, we are creating simple database with couple of small tables.

![image](https://user-images.githubusercontent.com/20516321/196590254-29b812c3-efdb-4ea8-9af8-d3d84a861fe3.png)


## Load Data

1. Open SSMS > Provide below info > Click on **Connect**

![image](https://user-images.githubusercontent.com/20516321/116333897-f25bee00-a7f1-11eb-8cd0-161a5ed8e4dc.png)
``` sql
CREATE DATABASE rritecDB;

GO

use rritecDB;

GO

CREATE TABLE [dbo].[DEPT]
(DEPTNO INT PRIMARY KEY ,
DNAME VARCHAR(20),
LOC VARCHAR(20) );

GO

INSERT INTO [dbo].[DEPT] VALUES (10, 'ACCOUNTING', 'NEW YORK');

INSERT INTO [dbo].[DEPT] VALUES (20, 'RESEARCH', 'DALLAS');

INSERT INTO [dbo].[DEPT] VALUES (30, 'SALES', 'CHICAGO');

INSERT INTO [dbo].[DEPT] VALUES (40, 'OPERATIONS', 'BOSTON');


CREATE TABLE [dbo].[EMP]
(EMPNO INT PRIMARY KEY,
ENAME VARCHAR(20),
JOB VARCHAR(20),
MGR INT,
HIREDATE DATE,
SAL MONEY,
COMM MONEY,
DEPTNO INT );

GO

INSERT INTO [dbo].[EMP] VALUES (7369, 'SMITH', 'CLERK', 7902, '17-DEC-1980', 800, NULL, 20);

INSERT INTO [dbo].[EMP] VALUES (7499, 'ALLEN', 'SALESMAN', 7698, '20-FEB-1981', 1600, 300, 30);

INSERT INTO [dbo].[EMP] VALUES (7521, 'WARD', 'SALESMAN', 7698, '22-FEB-1981', 1250, 500, 30);

INSERT INTO [dbo].[EMP] VALUES (7566, 'JONES', 'MANAGER', 7839, '2-APR-1981', 2975, NULL, 20);

INSERT INTO [dbo].[EMP] VALUES (7654, 'MARTIN', 'SALESMAN', 7698, '28-SEP-1981', 1250, 1400, 30);

INSERT INTO [dbo].[EMP] VALUES (7698, 'BLAKE', 'MANAGER', 7839, '1-MAY-1981', 2850, NULL, 30);

INSERT INTO [dbo].[EMP] VALUES (7782, 'CLARK', 'MANAGER', 7839, '9-JUN-1981', 2450, NULL, 10);

INSERT INTO [dbo].[EMP] VALUES (7788, 'SCOTT', 'ANALYST', 7566, '09-DEC-1982', 3000, NULL, 20);

INSERT INTO [dbo].[EMP] VALUES (7839, 'KING', 'PRESIDENT', NULL, '17-NOV-1981', 5000, NULL, 10);

INSERT INTO [dbo].[EMP] VALUES (7844, 'TURNER', 'SALESMAN', 7698, '8-SEP-1981', 1500, 0, 30);

INSERT INTO [dbo].[EMP] VALUES (7876, 'ADAMS', 'CLERK', 7788, '12-JAN-1983', 1100, NULL, 20);

INSERT INTO [dbo].[EMP] VALUES (7900, 'JAMES', 'CLERK', 7698, '3-DEC-1981', 950, NULL, 30);

INSERT INTO [dbo].[EMP] VALUES (7902, 'FORD', 'ANALYST', 7566, '3-DEC-1981', 3000, NULL, 20);

INSERT INTO [dbo].[EMP] VALUES (7934, 'MILLER', 'CLERK', 7782, '23-JAN-1982', 1300, NULL, 10);

INSERT INTO [dbo].[EMP] VALUES (1234, 'Ram', 'CLERK', 7782, '23-JAN-1982', 1400, NULL, 50);

GO

CREATE TABLE [dbo].[SALGRADE]
(GRADE INT NOT NULL,
LOSAL MONEY,
HISAL MONEY );

GO

INSERT INTO [dbo].[SALGRADE] VALUES (1, 700, 1200);

INSERT INTO [dbo].[SALGRADE] VALUES (2, 1201, 1400);

INSERT INTO [dbo].[SALGRADE] VALUES (3, 1401, 2000);

INSERT INTO [dbo].[SALGRADE] VALUES (4, 2001, 3000);

INSERT INTO [dbo].[SALGRADE] VALUES (5, 3001, 9999);
```

## Import tables(emp,dept and salgrade) into Power BI
---

1. Open **Power BI Desktop** > Click on **Get Data** > Click on **Databases** > select **SqlServer Database** > click on **connect**


 
1. provider server as **localhost** > Database as **rritecDB** > Click on **ok**

    
    
1. Select emp and dept tables > clcik on **LoadData** 

 
## Exercise:
- Do all exercise of [PBI_01_02_Power Query Editor Shape data using Excel as source](https://github.com/rritec/powerbi/blob/8cd3e9b6ff889c7056baf4c71b951dd152a41c16/Notebooks/PBI_01_02_Power%20Query%20Editor%20Shape%20data%20using%20Excel%20as%20input.md)

## Questioons
---
1. What is SSMS ?
 - SQL Server Management Studio (SSMS) is an IDE that provides a graphical interface for connecting and working with MS SQL server
2. How many rows inserted in emp table ?
 - 14 (select count(*) from [dbo].[emp])
3. Write SQL to get deptname wise salary expenditure?
 - select dnmae,sum(sal) from [dbo].[emp],[dbo].[dept] where emp.deptno=dept.deptno group by dname
4. Who is top sal employee?
 - King(5000)

#  optional

![image](https://user-images.githubusercontent.com/20516321/196850801-05c4bd18-3736-4328-b2dc-9288182d81be.png)


# M-Language

1. Power Query is a Formula Language (Informally known as "M")
2. **M** stands for **Mash-Up**
3. **M** is a case-sensitive language
4. Power Query is a data transformation and data preparation engine. Power Query comes with a graphical interface for getting data from sources and a Power Query Editor for applying transformations. Because the engine is available in many products and services, the destination where the data will be stored depends on where Power Query was used. Using Power Query, you can perform the extract, transform, and load (ETL) processing of data.

![image](https://user-images.githubusercontent.com/20516321/118579120-12584f00-b7ab-11eb-8f40-dee8dd8bfd24.png)

## Reference doc 

https://docs.microsoft.com/en-us/powerquery-m/quick-tour-of-the-power-query-m-formula-language

### Exercise 1: Write Simple M-languge Query

1. Open **Power BI Desktop** > Click on **Get Data** > Click on **Blank Query** > In **Power Query Editor** > Click on **Advanced Editor** > Then copy paste below code

``` F#
let
    x = 1 +1,
    y= 2+2,
    z = x+y+3
in
    z
```
1. Click on done
2. Click on apply and close
3. develop report and observe output
### Exercise 2: Write Simple M-languge Query with spaces in variable name.

1. Replace above code with below code and observe result

``` F#
let
        #"First Name" = "Ram",
        #"Last Name" = "Reddy",
        #"Full Name" = Text.Combine({#"First Name", #"Last Name"})
in
        #"Full Name"
```
            
            
 ### Exercise 3: Call functions in M-language

1. Replace above code with below code and observe result

``` F#
//this is a single line comment
/* This
is 
a
multiline
comment*/

let
   date = #date(2021,04,25),
   year = Date.Year(date)
in
    year
```
### Exercise 4: Real world example

1. Open any one PBIX file and observe M-language code
2. In screenshot below, you can see all basics mentioned so far:
        - **let** and **in** block
        - Variable names matching steps applied in the query
        - Some variable names with hashtag and double quote: #”var name”
        - End of the line characters: **comma**
        - Calling many functions
        ![image](https://user-images.githubusercontent.com/20516321/116349500-c77f9300-a80d-11eb-9559-0d88ac8890b5.png)

### Questions:
---
1. What is the result of below program

```F#
let 
        Sales2007 =  
        [  
            Year = 2007,  
            FirstHalf = 1000,  
            SecondHalf = 1100, 
            Total = FirstHalf + SecondHalf // 2100 
        ], 
        Sales2008 =  
        [  
            Year = 2008,  
            FirstHalf = 1200,  
            SecondHalf = 1300, 
            Total = FirstHalf + SecondHalf // 2500 
        ] 
in 
        Sales2007[Total] + Sales2008[Total]
```

2. What is the result of below program

```F#
let
        SimpleInterest = (p,t,r) => p*t*r/100,
        // Here 
        // p is principal
        // t is time in months
        // r is rate of interest
        rs = SimpleInterest(100,12,2)
in 
        rs
```

3. What is the result of below program

```F#
let
    a =
    [
        x = 1,       
        y = 2,       
        z = x + y    
    ], 
    b = 3             
in 
    a[z] + b         
```

4. What is the result of below program

```F#
let
    a = List.Contains({1, 2, 3, 4, 5}, 3),
    b = List.Contains({1, 2, 3, 4, 5}, 6)
in 
    {a,b}        
```

5. What is the result of below program

```F#
let
        rs = List.Select({1, -3, 4, 9, -2}, each _ > 0)
in 
        rs  
```

6. What is the result of below program

```F#
let
        rs = List.Sum({1, 2, 3})
in 
        rs
```
   


7. What is the result of below program

```F#
let
   student=Table.FromRecords(
    {
        [sno =101,sname="ram",scourse="powerbi",sfee=100],
        [sno =102,sname="nancy",scourse="powerapps",sfee=200],
        [sno =103,sname="john",scourse="powerautomate",sfee=300]
    }
       )
in
    student       

```
8. What is the result of below program

```F#
let
rs = Table.AlternateRows(
    Table.FromRecords({
        [CustomerID = 1, Name = "Bob", Phone = "123-4567"],
        [CustomerID = 2, Name = "Jim", Phone = "987-6543"],
        [CustomerID = 3, Name = "Paul", Phone = "543-7890"]
    }),
    1,1,1
)
in 
        rs       
```
9. What is the result of below program

```F#
let
        rs = Table.FuzzyGroup(
            Table.FromRecords(
                {
                    [EmployeeID = 1, Location = "Seattle"],
                    [EmployeeID = 2, Location = "seattl"],
                    [EmployeeID = 3, Location = "Vancouver"],
                    [EmployeeID = 4, Location = "Seatle"],
                    [EmployeeID = 5, Location = "vancover"],
                    [EmployeeID = 6, Location = "Seattle"],
                    [EmployeeID = 7, Location = "Vancouver"]
                },
                type table [EmployeeID = nullable number, Location = nullable text]
            ),
            "Location",
            {"Count", each Table.RowCount(_)},
            [IgnoreCase = true, IgnoreSpace = true]
        )
in 
        rs       
```

10. What is the result of below program

```F#
let
    startdate=DateTime.From(#date(2022, 1, 1)),
    enddate=DateTime.LocalNow(),
    numberofdays=Duration.Days(enddate-startdate),
    Dates = List.DateTimes(startdate, numberofdays+1, #duration(1,0,0,0)),
    #"Converted to Table" = Table.FromList(Dates, Splitter.SplitByNothing(), null, null, ExtraValues.Error),
    #"Renamed Columns" = Table.RenameColumns(#"Converted to Table",{{"Column1", "Date"}}),
    #"Changed Type" = Table.TransformColumnTypes(#"Renamed Columns",{{"Date", type datetime}}),
    #"Added Custom" = Table.AddColumn(#"Changed Type", "year", each Date.Year([Date])),
    #"Changed Type1" = Table.TransformColumnTypes(#"Added Custom",{{"year", Int64.Type}}),
    #"Added Custom1" = Table.AddColumn(#"Changed Type1", "monthnumber", each Date.Month([Date])),
    #"Added Custom2" = Table.AddColumn(#"Added Custom1", "Monthname", each Date.MonthName([Date])),
    #"Changed Type2" = Table.TransformColumnTypes(#"Added Custom2",{{"monthnumber", Int64.Type}, {"Monthname", type text}}),
    #"Added Custom3" = Table.AddColumn(#"Changed Type2", "daynumber", each Date.Day([Date])),
    #"Added Custom4" = Table.AddColumn(#"Added Custom3", "weeknumber", each Date.WeekOfYear([Date])),
    #"Changed Type4" = Table.TransformColumnTypes(#"Added Custom4",{{"weeknumber", Int64.Type}})
    
in
     #"Changed Type4"      
```
 



# Power Query Editor Combine Data


- In power BI, we can combine data intwo ways
	1. Append
	2. Merge
## Append
1. Rows appending
1. It is equal to sql union all
1. Append rules
	- Rule 1: The number of columns in each table should be same, other wise it will fill with null values.        
	- Rule 2: The respective columns data types shoud be same 
### Exercise 1: Append emp10,emp20 and emp30 tables as **emp102030**

#### Sql Query
- Create required tables

``` sql 
SELECT * INTO [dbo].[emp10] FROM [dbo].[EMP] WHERE DEPTNO=10;

SELECT * INTO [dbo].[emp20] FROM [dbo].[EMP] WHERE DEPTNO=20;

SELECT * INTO [dbo].[emp30] FROM [dbo].[EMP] WHERE DEPTNO=30;
```
	

- Verify data


```sql
select * from emp10 -- 3 rows
union
select * from emp20 -- 5 rows
union
select * from emp30 -- 6 rows
```
#### Difference between Union and Union all
- Observe Results of below Queries

``` sql 
select * from emp10 -- 3 rows
union
select * from emp10 -- 3 rows
```

``` sql 
select * from emp10 -- 3 rows
union all
select * from emp10 -- 3 rows
```
#### Intersection
- Observe Results of below Queries

``` sql 
select * from emp10 -- 3 rows
intersect
select * from emp10 -- 3 rows
```
``` sql 
select * from emp10 -- 3 rows
intersect
select * from emp20 -- 5 rows
```
#### except
- Observe Results of below Queries

``` sql 
select * from emp10 -- 3 rows
except
select * from emp10 -- 3 rows
```

#### Develop Report using Append homogeneous Sources

1. Open **Power BI** > Click on **Get Data** > Select **Databases**> Select **SqlServer** > Click on **Connect** > Provide **Servername** as **localhost** and **Database Name** as **rritec** > Click on **ok**
1. In **Navigator** window Select tables **emp10**,**emp20** and **emp30** > Click on **Transform Data**
1. Click on **Append Queries** > **Append Queries as New** > Select radio button **Three or More Tables** > Select required tables and push to right side then click on **ok**



### Develop Report using Append Hetrogeneous Sources

1. In above report import emp30 data from excel **LabData/Lab1/emp30_data_from_excel.XLSX**
1. Combine This Excel emp 30 with SQL Server emp10 data



## Merge
1. Inner Join
1. Left outer Join
1. Right Outer Join
1. Full Outer Join
1. Right Anti Join
1. Left Anti Join
1. Non Equi Join
1. Cross Join
1. Self Join


### Inner Join

#### Learn Sql Query

```sql
Select dname,ename,job,sal
from emp,dept
where emp.deptno=dept.deptno
```
	
OR 

``` sql
Select emp.deptno,dept.deptno,dname,ename,job,sal
from emp inner join dept
on emp.deptno=dept.deptno
```

#### Develop PBI Report using inner Join

1. In above Report import **emp** and **dept**
1. Click on **Merge Queries** > **Merge Queries as New** > Select Join Columns as shown below >Select Type of Join as **Inner Join** > click on **ok**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0033.png?raw=true)
1. In **Query Settings** rename **merge1** as **01_Inner_join**
1. Expand Dept Table in the **work Area** and **Select all columns** > Click on **ok** > Understand Result of SQL Query in database and powerI result, Both Must be same

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0034.png?raw=true)

### Left Outer Join

#### Learn Sql Query

``` sql
Select emp.deptno,dname,ename,job,sal
from emp left outer join dept
on emp.deptno=dept.deptno
```

#### Develop PBI Report using Left Outer Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **02_Left_outer_Join**
1. Click on  **Source** Settings and change **inner join** as **Left Outer Join** 
1. Click on **ok** 
1. Observe result
1. Notice that Ram Reddy record available even though he is belongs to 50 dept no

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0035.png?raw=true)

### Right Outer Join

#### Learn Sql Query

``` sql
Select dept.deptno,dname,ename,job,sal
from emp right outer join dept
on emp.deptno=dept.deptno
```

#### Develop PBI Report using Right Outer Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **03_Right_outer_Join**
1. Click on  **Source** Settings and change **inner join** as **Right Outer Join** 
1. Click on **ok** 
1. Observe Result

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0036.png?raw=true)

### Full Outer Join

#### Learn Sql Query

``` sql 
Select dept.deptno,dname,ename,job,sal
from emp left outer join dept
on emp.deptno=dept.deptno
union 
Select dept.deptno,dname,ename,job,sal
from emp right outer join dept
on emp.deptno=dept.deptno 
```

or 

``` sql
select dept.deptno,emp.deptno,dname,loc,empno,ename,sal
from [dbo].[EMP] full outer join [dbo].[DEPT]
on dept.deptno=emp.deptno 
```

#### Develop PBI Report using Full Outer Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **04_Full_outer_Join**
1. Click on  **Source** Settings and change **inner join** as **Full Outer Join** 
1. Click on **ok** 
1. Observe Result

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0037.png?raw=true)

### Left Anti Join

#### Learn Sql Query

``` sql 
select * from emp
where deptno not in (select deptno from dept );
```

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0038.png?raw=true)

#### Develop PBI Report using Left Anti Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **05_Left_Anti_Join**
1. Click on  **Source** Settings and change **inner join** as **Left Anti Join** 
1. Click on **ok** 
1. Observe Result

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0039.png?raw=true)

### Right Anti Join

#### Learn Sql Query

``` sql
select * 
from dept 
where deptno not in (select deptno from emp );
```

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0040.png?raw=true)

#### Develop PBI Report using Right Anti Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **06_Right_Anti_Join**
1. Click on  **Source** Settings and change **inner join** as **Right Anti Join** 
1. Click on **ok** 
1. Observe Result

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0041.png?raw=true)

### Non Equi Join

#### Learn Sql Query
``` sql
select ename,sal,grade 
from emp,salgrade 
where sal between losal and hisal
```

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0042.png?raw=true)

#### Develop PBI Report using Non Equi Join
1. Click on **Get Data** > Select **Databases**> Select **MySql** > Click on **Connect** > Provide **Servername** as **localhost** and **Database Name** as **rritec** > Click on **Advanced Options** > under **SQL Statement** ,paste above sql > Click on **ok**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0043.png?raw=true)
	
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0044.png?raw=true)
	
1. In **Query Settings** rename query as **Non Equi Join**
1. Observe result    

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0045.png?raw=true)

### Cross Join

#### Learn Sql Query
``` sql
select ename,dname,job,sal
from emp,dept
```

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0046.png?raw=true)

#### Develop PBI Report using Cross Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **05_Left_Anti_Join**
1. Click on  **Source** Settings and change **inner join** as **Left Anti Join** 
1. Click on **ok** 
1. Observe Result

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0047.png?raw=true)
    
#### Develop PBI Report using Self Join
``` sql
select e.ename as employee_name,m.ename as manager_name 
from emp as e,emp as m
where e.mgr=m.empno
```

## Home Work: Develop Below reports

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0022.png?raw=true)

## Questions
1. What is composite Key ?

	A composite key is a combination of two or more columns in a table that can be used to uniquely identify each row in the table
	
	![image](https://user-images.githubusercontent.com/20516321/127946905-78dea4ea-93aa-49da-9cff-0c72aaa38264.png)

	
	
1. Can we merge/Join in power bi with two or more columns?

	Yes. Press Ctrl key and select multiple columns.
	
	*Note:* In *Model* we can not create join based on multiple columns 
1. How many types of combine available in PowerBI?

	1. Append
	
	2. Merge
1. What you mean by append?

	Combining rows from two or more tables
1. What you mean by Merge?
	
	Merge is nothing but Join
1. How many types of Mergeing possible in Power BI?
	
	- 6 Types and those are 
		- Inner Join
		- Left Outer Join
		- Right Outer Join
		- Full Outer Join
		- Left Anti Join
		- Right Anti Join
1. Can you show null mesures coresponding rows in the report?
	No. As a work around we can replace NULL with something(like Zero,NA,...etc)
1. Understand below data and answer questions?
	- Table 1
	
	| Col1 | Col2 |
	| --- | --- |	
	| 101 | ram |	
	| 102 | raju |
	
	- Table 2
	
	| Col1 | Col2 |
	| --- | --- |	
	| 101 | Accounting |	
	| 102 | IT |
	
	1. if i create join between these two tables 
		- using **inner join** how many rows will get in result?
			- 2
		- using **left outer join** how many rows will get in result?
			- 2
		- using **right outer join** how many rows will get in result?
			- 2			
		- using **full outer join** how many rows will get in result?
			- 2	
1. Power BI **Append** works as **union** or **union all**?
	- Union all
1. What is the difference between **union** and **union all**
	- Union --> it will not produce duplicates rows
	- union all --> will produce duplicate rows




# Project1 Power Query Editor Lab

- **Power BI Desktop** Key Components
    1. Power Query Editor
        - Connecting Data Sources
            - Files(Excel ... etc)
            - Relational Databases (MySql,MS Sql Server ... etc)        - 
        - Import Tables
        - Transformations
            - Replace **null** with **zero**
            - Add new column
            - Change datatype
            - Filter data
            - .... etc        
        - Understanding Transformations in M-Language of Power BI
        - Combine
            - Append(Union All)
            - Merge(Join)
                - Inner Join
                - Left Outer Join
                - Right Outer Join
                - Full Outer JOin
                - Left Anti Join
                - Right Anti Join 
        - Based on these concepts let us do one small project
    1. Power Pivot
    1. Power View
    
# Lab Overview

## SCENARIO
ABC is a company that manufactures and sells **sporting goods**. The company has offices in the United States (US) and several other countries. Its sales comprise of US sales and International sales. ABC’s sales come from its owned manufactured products, as well as other manufacturers’ products.

ABC's US office stores the sales data on an **Access** database. ABC International sales transactions are available as **Comma Separated Values (CSV)** files. They could be generated daily, either manually by someone, or automatically by an automated process. They are available in a dedicated folder. These CSV files have the same column structure as the sales table for the US sales that comes from the SQL Database.

You want to perform analysis on ABC's worldwide sales data for the year **2000 to 2015**. You need to bring all these data into Power BI Desktop before you can perform any analysis. Finally, you want to compare ABC's **country sales with the country population**. You need to import the country population data from a less structured **Excel** report to Power BI.



## LAB OVERVIEW

This lab comprises of three exercises:

In the **First Exercise**, you will import data to Power BI Desktop from an Access database file.

In the **Second Exercise**, you will import data from CSV files which resides in a file folder. You will append this new data to the corresponding existing data that comes from the Access Database.

In the **Third Exercise**, you will import data to Power BI Desktop from an Excel file that is less structured.



## WHAT YOU'LL NEED

A computer with the latest version of Power BI Desktop installed on it.

A copy of the `Access Database` containing ABC's US sales data.

`4 CSV files`, containing ABC’s international sales data:

1. CA Sales.csv
2. FR Sales.csv
3. DE Sales.csv
4. MX Sales.csv

An `Excel` file containing country population data.

## Import Data from Access Database


1. Open `Power BI Desktop`.
2. Click `Get Data`.
3. Click `Access database`, and click `Connect`.
4. Navigate to `LabData`, click `PowerBI.accdb`, and click `Open`.
5. Select `bi_date, bi_geo, bi_manufacturer, bi_product` and `bi_salesFact` and click `Transform`.
6. In Queries, select `bi_salesFact`.
7. Select the `Date` column.
8. Click the `Transform` ribbon.
9. In the `Any Column` group, select `Data Type` and select `Date`.
10. Click the drop-down button at the top of the `Date` column.
11. Click `Date` Filters and click `After`.
12. In the first Enter or select a value field, type 12/31/1999 if you are using MM/DD/YYYY dates and 31/12/1999 if you are using DD/MM/YYYY dates and click OK.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0092.png?raw=true)
    
13. In `Queries`, select `bi_Date`.
14. Select the Date column.
15. Click the Transform ribbon.
16. In the Any Column group, select Data Type and select Date.
17. Click the drop-down button at the top of the Date column.
18. Click Date Filters and click After.
19. In the first Enter or select a value field, type 12/31/1999 if you are using DD/MM/YYYY dates and 31/12/1999 if you are using DD/MM/YYYY dates and click OK.
20. Rename the queries as follows:

- In Queries, right click **bi_date**, click Rename, replace the text with **Date**, and press Enter.
- In Queries, right click **bi_geo**, click Rename, replace the text with **Locations**, and press Enter.
- In Queries, right click **bi_manufacturer**, click Rename, replace the text with **Manufacturers**, and press Enter.
- In Queries, right click **bi_product**, click Rename, replace the text with **Products**, and press Enter.
- In Queries, right click **bi_salesFact**, click Rename, replace the text with **Sales**, and press Enter.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0094.png?raw=true)
    
21. Click the Home ribbon.
22. Click **Close and Apply**.
23. Click **Data** and explore the imported data in the Data View.

## Import Data from a Folder Containing CSV Files

Continue with your Power BI file from the previous exercise. You want to create a Query for the International sales and append the Query to the Query from US Sales.

1. On the **Home** ribbon, click **Get Data** > click **File** > Click **Folder** > click **Connect**.
1. In Folder path, go to **labdata/Lab1** and select **International** folder, and click **OK**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0095.png?raw=true)

1. Click on **Combine & Transform Data**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0096.png?raw=true)

1. Observe data > Click on **ok**
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0097.png?raw=true)    

1. In **QUERY SETTINGS** change the name to **International Sales**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0098.png?raw=true) 
    
1. Select the **Date** column.
1. Click the **Transform** ribbon.
1. In the **Any Column** group, select **Data Type** and select **Date**.
1. Click the drop-down button at the top of the **Date** column.
15. Click **Date Filters** > click **After**.
16. In the first Enter or select a value field, type **12/31/1999** if you are using DD/MM/YYYY dates
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0099.png?raw=true)
    
17. In **Queries**, select **Sales**.
18. On the **Home** ribbon, click **Append Queries**.
19. Select **International Sales** and click **OK**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0100.png?raw=true)
    
20. On the **Add Column** ribbon > Click on **Custom Column**.
21. In New column name type **Country Name**.
22. To replace null values with USA, in Custom column formula, type the following formula and click OK:
`=if [Country] = null then "USA" else [Country]`
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0101.png?raw=true)
    
    
23. Right-click the header of the **Country** column and click **Remove**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0102.png?raw=true)
    
24. Click the **Home** ribbon.
25. Click **Close & Apply**.
26. Click **Data** and explore the imported data in the **Data View**.

## Import a Less Structured Data from an Excel File
 

Continue with your Power BI file from the previous exercise. You want to import an Excel report containing population data for the countries that VanArsdel operates.

1. Import the data from the file folder by clicking **Get Data** > **Excel** > **Connect**.
1. Select **..Labdata/lab1/Country Population by Year.xlsx** and click **Open**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0103.png?raw=true)

1. Select **Sheet1** and click **Transform Data**.
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0104.png?raw=true)    
    
1. In **QUERY SETTINGS** change Name to **Country Population**.
1. On the ribbon, click **Remove Rows** > Click **Remove Top Rows** > in **Number of rows** >  type **3** > click **OK**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0105.png?raw=true)
    
1. On the ribbon, click Use **First Row as Headers**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0106.png?raw=true)    
1. Select the **1999** column, hold **Shift** and select the **2014** column.
1. On the **Transform** ribbon, click **Unpivot** Columns.
1. Right-click the **Attribute** column header and click **Rename**.
1. Type **Year** and press **Enter**.
1. Right-click the **Value** column header and click **Rename**.
1. Type **Population** and press **Enter**.
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0107.png?raw=true)
    
1. Click the **drop-down** button on the **Year** header, unselect **1999**, and click **OK**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0108.png?raw=true)
    
1. Click the **Year** header, on the **Transform** ribbon click **Data Type**, and click **Whole Number**.
1. Click the **Population** header, on the **Transform** ribbon click **Data Type**, and click **Whole Number**.
1. Click the **Home** ribbon.
1. Click **Close & Apply**.
1. Load the **data** into Power BI Desktop.
1. Explore the imported data in the Data View.


## Questions
-----
1. How Many Types of connections available in **Power BI**
    - Import
    - DirectQuery
    - Live Connection
    - Streaming Connection
2. What is difference between Import and Direct Connection?
    1. Import:
        - Gives you the **full suite** of transformation and **data manipulation** in the Desktop
        - There is a 1 GB limit to the Desktop if you plan on publishing to the PBI Service
        - Scheduling Datasets using gateway is needed to avoid old(stale) data
    2. DirectQuery:
        - Limits your ability to manipulate data in the Desktop (removes the Data section)
        - Leaves the data in the SQL database
        - Is "live", no need to schedule a refresh (In the Service)
2. What is the max data limit in a given dataset?

    - **1 GB**
    
    - for more information read this [doc](https://docs.microsoft.com/en-us/power-bi/admin/service-admin-manage-your-data-storage-in-power-bi#:~:text=There%20is%20a%201%20GB,250%20MB%20for%20the%20dataset)
1. How Power BI define datatypes?
    - Based on first 200 rows data values


```python

```

#  Power Query Editor Knowledge Test

https://docs.google.com/forms/d/e/1FAIpQLScXps5bMocuSuFrZCaZ3iSsDqDW_N79INcdFzHGEc_Cug6NZQ/viewform?usp=sf_link

https://docs.google.com/forms/u/2/d/1eHMES9qZATaOuvpYy3X2ewBDRm3flJt-CGFCahR6tac/edit


# Power Pivot Modeling Part1
  - It is useful to do two activities  
    1. Modeling
        - Relation ship(Among Tables) Vs Join(Among Queries)
        - Cardinality
          - One to One
          - One to Many
          - **Many to One**(Default)
          - Many to Many
        - Cross Filter Directions
          - **Single**(Default)
          - Both
        - Active Vs Inactive Relationships   
    - Note: Please listen first *three videos*    https://rritec.blogspot.com/p/obiee.html
    2. DAX Calculations  
## Exercise 1: Create Two tables using Enter Data Method
1. When you import multiple tables, chances are you'll do some analysis using data from all those tables. Relationships between those tables are necessary to accurately calculate results and display the correct information in your reports.
2. Power BI Desktop makes creating those relationships easy. In fact, in most cases you won’t have to do anything, the autodetect feature does it for you based on common column names and data.
3. The first table, **ProjectHours**, is a record of work tickets that record the number of hours a person has worked on a particular project. 
4. Open **Power BI Desktop** > In the toolbar click on **Enter Data** > Provide **Table Name** as **ProjectHours** > copy below data and paste into workspace

    | **Ticket** | **SubmittedBy** | **Hours** | **Project** | **DateSubmit** |
    | ---:|:--- | ---:|:--- | ---:|
    | 1001 |Brewer Alan |22 |Blue |1/1/2013 |
    | 1002 |Brewer Alan |26 |Red |2/1/2013 |
    | 1003 |Ito Shu |34 |Yellow |12/4/2012 |
    | 1004 |Brewer Alan |13 |Orange |1/2/2012 |
    | 1005 |Bowen Eli |29 |Purple |10/1/2013 |
    | 1006 |Bento Nuno |35 |Green |2/1/2013 |
    | 1007 |Hamilton David |10 |Yellow |10/1/2013 |
    | 1008 |Han Mu |28 |Orange |1/2/2012 |
    | 1009 |Ito Shu |22 |Purple |2/1/2013 |
    | 1010 |Bowen Eli |28 |Green |10/1/2013 |
    | 1011 |Bowen Eli |9 |Blue |10/15/2013 |

5. This second table, **CompanyProject**, is a list of projects with an assigned priority: A, B, or C. Create this table also simillar to above table.

    | **ProjName** | **Priority** |
    | --- | --- |
    | Blue |A |
    | Red |B |
    | Green |C |
    | Yellow |C |
    | Purple |B |
    | Orange |C |
6. Notice that each table has a **project** column. Each is named slightly different, but the values look like they’re the same.
## Exercise 2: Number of hours submitted by project priority without relationship
1. Select **Priority** and **Hours** from the **Fields** pane.  
2. If we look at our table in the report canvas, you’ll see the number of hours is 256 for each project, which is also the total. Clearly this number isn’t correct. Why? It’s because we can’t calculate a sum total of values from one table (**Hours** in the **Project** table), sliced by values in another table (**Priority** in the **CompanyProject** table) without a relationship between these two tables.
## Exercise 3: Number of hours submitted by project priority with relationship
7. Go to model and create relation using **ProjName** and **project** columns
8. Come to report observe the data.
## Exercise 4: Understand Role Playing Dimension and solutions to reslove the issue of Role Playing Dimension

7. Open **Power BI Desktop** > In the toolbar click on **Enter Data** >
8. Click on **Enter Data** > create below tables

  **ProjectTickets**

| Ticket	| OpenedBy	| SubmittedBy	| Hours	| Project	| DateSubmit |
| --- | --- | --- | --- | --- | --- |
| 1001	| Perham, Tom	| Brewer, Alan | 22	| Blue	| 1/1/2013 | 
| 1002	| Roman, Daniel |	Brewer, Alan | 26 |	Red |	2/1/2013 |
| 1003	| Roth, Daniel |	Ito, Shu |	34 |	Yellow |	12/4/2012 |
| 1004	| Perham, Tom |	Brewer, Alan |	13 |	Orange |	1/2/2012 |
| 1005	| Roman, Daniel |	Bowen, Eli |	29 |	Purple |	10/1/2013 |
| 1006	| Roth, Daniel |	Bento, Nuno |	35 |	Green |	2/1/2013 |
| 1007	| Roth, Daniel | Hamilton, David |	10 | Yellow | 10/1/2013 |
| 1008	| Perham, Tom |	Han, Mu |	28 |	Orange |	1/2/2012 |
| 1009	| Roman, Daniel |	Ito, Shu |	22 |	Purple |	2/1/2013 |
| 1010	| Roth, Daniel |	Bowen, Eli |	28 |	Green |	10/1/2013 |
| 1011	| Perham, Tom |	Bowen, Eli |	9	| Blue | 10/15/2013|

**EmployeeRole**

  | **Employee** | **Role** |
  | --- | --- |
  | Bento, Nuno |Project Manager |
  | Bowen, Eli |Project Lead |
  | Brewer, Alan |Project Manager |
  | Hamilton, David |Project Lead |
  | Han, Mu |Project Lead |
  | Ito, Shu |Project Lead |
  | Perham, Tom |Project Sponsor |
  | Roman, Daniel |Project Sponsor |
  | Roth, Daniel |Project Sponsor |

## Exercise 5: Develop below report
1. Think and create relations and get below output.

![image](https://user-images.githubusercontent.com/20516321/150071049-e7050e74-2c3e-4425-8fe4-60db6d951d69.png)


# Power Pivot Modeling Part2
## Exercise: Single and Both Directions
1. A **Single-directional** relationship is one that filters in **one** directions.
1. A **bi-directional** relationship is one that filters in **both** directions.
1. By default relationship is **Single-directional**
1. Generally, we recommend minimizing the use of bi-directional relationships.
    - They can **negatively** impact on model query **performance**.

6. Follow MSFT [doc](https://docs.microsoft.com/en-us/power-bi/guidance/relationships-bidirectional-filtering)
## Reference
https://docs.microsoft.com/en-us/power-bi/desktop-create-and-manage-relationships
https://docs.microsoft.com/en-us/archive/blogs/cansql/relationships-in-power-bi-fixing-one-of-the-columns-must-have-unique-values-error-message

## Questions
----
1. What is composite models ?
  
    A model that combines data from more than one DirectQuery source or that combines DirectQuery with import data is called a composite model

    For more information refer [doc](https://docs.microsoft.com/en-us/power-bi/transform-model/desktop-composite-models#:~:text=A%20model%20that%20combines%20data,tables%20come%20from%20different%20sources.)

2. How many carinality's available?
  - One to One
  - One to Many
  - Many to One
  - Many to Many
    - Old versions of Power BI not supported. 
3. Fact to Dim what type of cardinality possible?
  - Many to One
4. Without Relationship, between two tables,will we get right data?
  - Wrong Data
5. Power BI creats relationships automatically based on what?
  - Column Names
6. Can you create Joins manually if column names are different?
  - Yes
7. Explain Single Vs Bi-directional Filters?
  - https://docs.microsoft.com/en-us/power-bi/guidance/relationships-bidirectional-filtering
8. What are the disadvantage of Bi-directional Join?
  - Negatively impact on model query performance
  - User confusing experiences
9. When to go for Bi-Directional Join? or Advantages of Bi-directional?
  - Special model relationships
    - one to one cardinality tables
    - Many to Many Cardinality Tables
    - **Note:** 99.99% we will have many to one relation tables in any dataset
  - Slicer items "with data"
  - Dimension-to-dimension analysis
  
  
# Power Pivot DAX Metrics


# Power Pivot

## Data Analysis eXpressions (DAX):
1. Data Analysis eXpressions (DAX) is a library of functions and operators that can be combined to build formulas and expressions in 
    - Power BI Desktop
    - Azure Analysis Services
    - SQL Server Analysis Services
    - Power Pivot in Excel data models.
1. Refer below MSFT Materials
    - [Help Document](https://docs.microsoft.com/en-us/dax/)
    - [Guided Learning Path](https://docs.microsoft.com/en-us/learn/paths/dax-power-bi/)

## DAX Functions mainily catagorized as below

    - Aggregation functions
    - Date and time functions
    - Filter functions
    - Financial functions 
    - Information functions
    - Logical functions
    - Math and Trig functions
    - Other functions
    - Parent and Child functions
    - Relationship functions
    - Statistical functions
    - Table manipulation functions
    - Text functions
    - Time intelligence functions

## Exercise 1: Learn Calendar function

1. Open PBI Desktop
1. In left side Navigation bar > Click on **Data**
1. Click on New Table
1. Provide DAX formula as **dt_table = CALENDAR (DATE (2019, 1, 1), DATE (2020, 12, 31))**
1. Create **new column** to extract **year**
2. Create **new column** to extract **month**
3. Create **new column** to extract **weeknumber**
4. Create **new column** to extract **day**
5. Create **new column** to extract **dayname**
    - **Hint:** Use Format Dax function [Refer help document](https://docs.microsoft.com/en-us/dax/format-function-dax#custom-datetime-formats)
7. Create **new column** to extract **end_of_the_month**
8. Create **new column** to extract **hour**
9. Create **new column** to extract **minute**
10. Create **new column** to extract **Second**

## Exercise 2: How many years survived by Mahatma Gandhi?

- We know Gandhi Born on October 2, 1869, and Died on January 30, 1948
- Read help document and find out no of years survived by Gandhi

    https://docs.microsoft.com/en-us/dax/datediff-function-dax
 - Process:
    - In Fields pane > Click on dt_table ... > click on new mesure > type the formula **Number of years survived = datediff(date(1869,10,02),date(1948,01,30))** > click on validate > drag this column into table and observe the output.

## Exercise 3: Using Variables to improve performance
- Any calculation, we are using twice or more better to store the calculation result in variable and use the variable where ever needed.
- Open [Adventure Works DW 2020 M02](https://github.com/rritec/powerbi/raw/master/Labdata/Adventure%20Works%20DW%202020%20M02.pbix) file
- Observe Calculation inside **Sales** table **Revenue YoY %**
- The last year sales, calculating two times right .
- Develop one mesure with the name of **Revenue YOY % using Var** with below formula

    ```
    Revenue YoY %_var =     
    VAR LySales = CALCULATE([Revenue],SAMEPERIODLASTYEAR('Date'[Date]))
    RETURN
    if(HASONEVALUE('Date'[Fiscal Year]),DIVIDE([Revenue]-LySales,LySales))
    ```
- Develop report as shown below
    - ![image](https://user-images.githubusercontent.com/20516321/147716190-3778224e-e457-4198-ae42-7a6d1fd08f7c.png)


## Exercise 4: Duplicate Table
- In Which scenario duplication of table isneeded?
    - Role Playing Dimension
- Open [Adventure Works DW 2020 M03](https://github.com/rritec/powerbi/raw/master/Labdata/Adventure%20Works%20DW%202020%20M03.pbix)
- In the Data view > Click on New Table > type below formula 

    ```
    Ship Date = 'Date'
    ```
- To complete the design of the Ship Date table, you can:
    - Rename the following columns:
        - **Date** as **Ship Date**
        - **Fiscal Year** as **Ship Fiscal Year**
        - **Fiscal Quarter** as **Ship Fiscal Quarter**
        - **Month** as **Ship Month**
        - **Full Date** as **Ship Full Date**
    - Sort the **Ship Full Date** column by the **Ship Date** column.
    - Sort the **Ship Month** column by the **MonthKey** column.
    - Hide the **MonthKey** column.
    - Create a hierarchy named Fiscal with the following levels:
        - Ship Fiscal Year
        - Ship Fiscal Quarter
        - Ship Month
        - Ship Full Date
    - Mark the **Ship Date** table as a date table by using the Ship Date column.

## Exercise 5: Can you populate dates of india financial year
- The financial year of India begins from April 1 of a calendar year and ends on March 31 of the next calendar year
- https://en.wikipedia.org/wiki/Fiscal_year
- In above PBIX file, develop a table report to understand range of dates

  ![image](https://user-images.githubusercontent.com/20516321/111573915-72de0680-87d1-11eb-8895-158a5d895da2.png)

- In the Data view > Click on New Table > type below formula 

    ```
    India Fin Dates =  CALENDARAUTO(3)
    ```
 - Using **India Fin Dates** Table **Date** Column  develop below report and understand how the Calendar Auto working.

   ![image](https://user-images.githubusercontent.com/20516321/111574107-d831f780-87d1-11eb-83ca-9b1254d9e1ff.png)

 - Read the [doc](https://docs.microsoft.com/en-us/dax/calendarauto-function-dax)



## Questions
1. About USERNAME() and USERPRINCIPALNAME()?
    - https://docs.microsoft.com/en-us/dax/username-function-dax
    - https://docs.microsoft.com/en-us/dax/userprincipalname-function-dax
    - In PowerBI Desktop
        - ![image](https://user-images.githubusercontent.com/20516321/109728973-34dfc080-7bdd-11eb-8dbb-ad4fd8316da4.png)
    - In Power BI Service
        - ![image](https://user-images.githubusercontent.com/20516321/109729142-740e1180-7bdd-11eb-9ec5-25db46bfd2cf.png)
        
 1. What is User Principal Name?
    - User Principal Name (UPN) is the name of a system user in an email address format.
    - A UPN (for example: john.doe@domain.com) consists of the user name (logon name), separator (the @ symbol), and domain name (UPN suffix)
  
1. What is Implicity Mesure.
    - Implicit measures are automatic behaviors that allow visuals to summarize model column data. 
1. What is Explicity Mesure.
    - Explicit measures, also known simply as measures, are calculations that you can add to your model.
1. What is compound Mesure.
    - When a measure references one or more measures, it's known as a compound measure.
    - Example ``` Profit = [Revenue] - [Cost] ```

1. Calculated columns Vs measures

    - DAX beginners often experience a degree of confusion about calculated columns and measures. The following section reviews the similarities and differences between both.
        - Regarding similarities between calculated columns and measures, both are:
            - Calculations that you can add to your data model.
            - Defined by using a DAX formula.
            - Referenced in DAX formulas by enclosing their names within square brackets.
        - The areas where calculated columns and measures differ include:
            - **Purpose** - Calculated columns extend a table with a new column, while measures define how to summarize model data.
            - **Evaluation** - Calculated columns are evaluated by using row context at data refresh time, while measures are evaluated by using filter context at query time. Filter context is introduced in a later module; it's an important topic to understand and master so that you can achieve sophisticated summarizations.
            - **Storage** - Calculated columns (in Import storage mode tables) store a value for each row in the table, but a measure never stores values in the model.
            - **Visual use** - Calculated columns (like any column) can be used to filter, group, or summarize (as an implicit measure), whereas measures are designed to summarize.


 


```python

```
# DAX iterator Functions

# Use aggregation iterator functions

- Each single-column summarization function has its equivalent iterator function.
- Example sum > sumx, min > minx, max > maxx, rank >rankx, count>countX, counta > countaX ..etc
- All scenarios of sum/min/max ..etc can also achivable using respective sumX/minX/maxX.... etc, however first priority goes to sum/min/max ..etc



## What is the difference between SUM() Vs SUMX()?
   - https://exceleratorbi.com.au/use-sum-vs-sumx/   
   - SUM() operates over a **single column** and has no awareness of individual rows in the column (no row by row evaluation).
   - SUMX() can operate on **multiple columns** in a table and can complete row by row evaluation in those columns.
   - SUMX() vs SUM(): Which One Should I Use?
      - Which you use really depends on your personal preference and the **structure of your data**.
      - In below example what we should use ?
      
      | product  | Quantity | Unit Price |        
      | ------------- | ------------- | -------- |        
      | Product 1 |	2	| 100 |        
      | Product 2 |	4	| 120 |        
      | Product 3 |	8 |	130 |
      
      - Answer is : Sumx
      - In below example what we should use ?
      
      
      | product  | Total Price |        
      | ------------- | -------- |        
      | Product 1 |	200 |        
      | Product 2 |	480 |        
      | Product 3 |	1040|
      
      
      - Answer is sum

   ### Process Steps:
   ----
   -  From SQL Server **Adventureworksdw2012** > Import **FactInternetSales** and **Customer** Table
   -  Observe the **Model** Relationship based on **customerkey** automatically created
   -  Creat a table vizulization with three columns **English Education**,**TotalProductCost**,**SalesAmount**
   -  ![image](https://user-images.githubusercontent.com/20516321/168948738-e6c7985b-f620-4e4d-aeba-bf0529b7ea61.png)

   -  Create **Margin** Mesure using below formula
   
           Margin = sumx(FactInternetSales,FactInternetSales[SalesAmount]-FactInternetSales[TotalProductCost])
   -  Create **TotalMargin** Mesure using below formula
   
            TotalMargin = sumx(all(FactInternetSales),FactInternetSales[SalesAmount]-FactInternetSales[TotalProductCost])
   -  Create **% Margin Contribution** Mesure using below formula
   
            % Margin Contribution = DIVIDE([Margin],[TotalMargin])
   -  Select **% Margin** > Change format as **Percentage**
   -  For more information Follow below blog and Develop below report
   - [Reference](https://radacad.com/sum-vs-sumx-what-is-the-difference-of-the-two-dax-functions-in-power-bi)
      ![image](https://user-images.githubusercontent.com/20516321/117744290-065a1380-b226-11eb-971f-87b9c80729a0.png)

## Calculate ranks

```sql

select e.*,
sum(sal) over ( partition by deptno),
rank() over(order by sal) as rank1,
dense_rank() over(order by sal) as denserank
from emp as e
order by deptno
```

- The RANKX DAX function is a special iterator function you can use to calculate ranks. Its syntax is as follows:
```RANKX(<table>, <expression>[, <value>[, <order>[, <ties>]]])```
- Ref Help [doc](https://docs.microsoft.com/en-us/dax/rankx-function-dax)
- Similar to all iterator functions, you must pass in a table and an expression. Optionally, you can pass in a rank value to find the order direction or to help you determine how to handle ranks when values are tied.

## Order direction
- Order direction is either ascending or descending.
- When ranking something favorable, like revenue values, you're likely to use descending order so that the highest revenue will be ranked first. 
- When ranking something unfavorable, like customer complaints, you might use ascending order so that the lowest number of complaints will be ranked first. 
- When you don't pass in an order argument, the function will use descending order.

## Handle ties
- You can handle ties by skipping rank values or using dense ranking, which uses the next rank value after a tie. 
- When you don't pass in a ties argument, the function will use skipped. 
- You'll have an opportunity to work with an example of each tie argument in subsequent sections.

## Create ranking measures
- Download [file](https://github.com/rritec/powerbi/raw/master/Labdata/Adventure%20Works%20DW%202020%20M05.pbix)
- Open file 
- Add the following measure 

  ```Product Quantity Rank = RANKX(ALL('Product'[Product]),[Quantity])```

- Add the Product Quantity Rank measure to the table visual that is found on Page 2 of the report. The table visual groups bike products and displays quantity, which orders products by descending quantity.
- The RANKX function iterates over a table that is returned by the ALL DAX function. The ALL function is used to return all rows in a model table or values in one or more columns, and it ignores all filters. Therefore, in this case, it returns a table that consists of all Product column values in the Product table. The RANKX function must use the ALL function because the table visual will group by product (which is a filter on the Product table).
- In the table visual, notice that two products tie for tenth place and that the next product's rank is 12. This visual is an example of using the Skipped ties argument.
- Bike Sales table visual with columns: Product, Quantity, and Rank, ordered by Quantity descending.
![image](https://user-images.githubusercontent.com/20516321/110742032-a7931080-825b-11eb-9bd3-40a885fb958e.png)

- Your next task is to enter the following logic to modify the Product Quantity Rank measure definition to use dense ranking:

  ``` Product Quantity Rank =RANKX(ALL('Product'[Product]),[Quantity],,,DENSE)```

- In the table visual, notice that a skipped ranking no longer exists. After the two products that tie for tenth place, the next ranking is 11.
- Bike Sales table visual with columns: Product, Quantity, and Rank, ordered by Quantity descending, but with dense ranking.
    ![image](https://user-images.githubusercontent.com/20516321/110742454-67805d80-825c-11eb-82e1-752da4ebc908.png)

- Notice that the table visual total for the Product Quantity Rank is one (1). The reason is because the total for all products is ranked.
- An image shows the Product Quantity Rank total is 1.
- It's not appropriate to rank total products, so you will now use the following logic to modify the measure definition to return BLANK, unless a single product is filtered:
  ```Product Quantity Rank = IF(HASONEVALUE('Product'[Product]),RANKX(ALL('Product'[Product]),[Quantity],,,DENSE))```
- An image shows the Product Quantity Rank total is BLANK.
  ![image](https://user-images.githubusercontent.com/20516321/110742868-20df3300-825d-11eb-888b-5f11d71d8857.png)

- Notice that the total Product Quantity Rank is now BLANK, which was achieved by using the HASONEVALUE DAX function to test whether the Product column in the Product table has a single value in filter context. It's the case for each product group, but not for the total, which represents all products.

**Home work:** [Top N dynamic selections](https://github.com/rritec/powerbi/blob/566b75a3a5850984fc9a9d9549104ce3dd70befe/Notebooks/Interview%20Questions/Top%20N%20Dynmic%20Selecton%20using%20what%20if%20parameter.md)

## Count Vs counta & count vs countx & counta vs countax
  - Enter below data and create a table

      | Employee Name | Date  | Holiday Flag | phone |        
      | ------------- | ------------- | ------------- | -------- |        
      | Ram | 01-Jan-2016 |	False	| 9573707079 |        
      | John | 02-Jan-2017 |	True	|  |        
      | Nancy | 01-Jan-2019 |	False |	1234567890 |

  - Make sure datatypes are Employee Name --> Text, Date --> Date , Holiday Flag --> Bool, Phone --> Whole Number
  - Can you count Date column using count and counta function?
      - yes
  - can you count bool column with count function?
      - No
  - Can you count bool column with counta?
      - Yes

  - count number of rows when holiday flag is *False*
      - *Hint*: use below formula inside the measure 
      - COUNTAX(FILTER(count_understanding,count_understanding[Holiday Flag]=FALSE()),count_understanding[Holiday Flag])  



#  DAX Studio

## About

- DAX Studio is a tool to write, execute, and analyze DAX queries in Power BI Desktop, Power Pivot for Excel, and Analysis Services Tabular.

## Setup environment 
1. Download DAX Studio Software [here](https://daxstudio.org/)
2. Double click on DAX STUDIO > Install it.
3. Download sample pbix file to follow dax studio tutorial https://github.com/microsoft/powerbi-desktop-samples/raw/main/DAX/Adventure%20Works%20DW%202020.pbix 
4. Open the above Power BI file
5. Go to Power BI Desktop > External Tools > Click on DAX Studio
## Tutorial 
7. Follow blog https://daxstudio.org/tutorials/writing-dax-queries/
### How to query a table of data?
Syntax: Evaluate \<Table Expression\>
       
        EVALUATE customer
More Examples:

        EVALUATE CALENDAR(date(2021,10,01),date(2021,10,05))
        EVALUATE FILTER(Customer,Customer[City]="Concord") 
        EVALUATE CALCULATETABLE(Customer,Customer[City]="Concord")
### How to query a table or column of data?
Syntax: VALUES\<tablename or columnname\>
        
        EVALUATE VALUES(Customer)
        EVALUATE VALUES(Customer[City])
        EVALUATE CALCULATETABLE(VALUES(Customer[City]),LEFT(Customer[City],1)="C")
        EVALUATE FILTER(VALUES(Customer[City]),LEFT(Customer[City],1)="C")

### How to sort the data?
Syntax: ORDER BY \<column names\> ASC/DESC
        
        EVALUATE CALCULATETABLE( VALUES ( Customer[City] ), LEFT ( Customer[City], 1 ) = "R" ) ORDER BY Customer[City]
        
### Returning a single value?

        
        EVALUATE { SUM ( Sales[Sales Amount] ) }
               
 ### Selecting columns from multiple tables?

        
        EVALUATE
        SUMMARIZECOLUMNS (
            Product[Color],
            Reseller[Business Type],
            FILTER ( ALL ( Product[List Price] ), Product[List Price] > 150.00 ),
            TREATAS ( { “Accessories”, “Bikes” }, ‘Product’[Category] ),
            “Total Sales”, SUM ( Sales[Sales Amount] )
        )
        
### Multiple Resultsets?

        
        EVALUATE Customer
        EVALUATE Product       

### Using Parameters in Queries?

        
        EVALUATE FILTER ( 'Product', 'Product'[Color] = @color_name )
        

### Write Dax Queries by comparing SQL Queries

// select * from Customer
//EVALUATE Customer

// select city from customer
//EVALUATE VALUES(Customer[City])

// select * from customer where city ="redmond"
//EVALUATE CALCULATETABLE ( Customer, Customer[City] = "Redmond" )

// select city  from customer where city like "R%"
//EVALUATE CALCULATETABLE(VALUES(Customer[City]),left(Customer[City],1)="R")

// select *  from customer where city like "R%"
//EVALUATE CALCULATETABLE(Customer,left(Customer[City],2)="Ro")

// select city  from customer where city like "R%" order by city desc
//EVALUATE CALCULATETABLE(VALUES(Customer[City]),left(Customer[City],1)="R") ORDER BY Customer[City] desc

![image](https://user-images.githubusercontent.com/20516321/169445380-cf011b56-3c7c-485f-bdc4-ced3857f1dc3.png)


### Exercise: Create a tabe in powerBI using below dax query
1. In DAX studio write below Dax query, run it  and understand result. 

        EVALUATE SUMMARIZECOLUMNS (
              Product[Color],
              Reseller[Business Type],
              FILTER ( ALL ( Product[List Price] ), Product[List Price] > 150.00 ),
              TREATAS ( { "Accessories", "Bikes" }, 'Product'[Category] ),
              "Total Sales", SUM ( Sales[Sales Amount] )
          )
2. Once we are happy with result then create table inside PBI
3. open PBI Desltop > data page
4. click on Dax Table, write below dax formula

        test_table_name =
          SUMMARIZECOLUMNS (
              Product[Color],
              Reseller[Business Type],
              FILTER ( ALL ( Product[List Price] ), Product[List Price] > 150.00 ),
              TREATAS ( { "Accessories", "Bikes" }, 'Product'[Category] ),
              "Total Sales", SUM ( Sales[Sales Amount] )
          )
5. Observe result

 ### More Examples

Explore online dax examples https://dax.guide/
Compare SQL to DAX Query examples  https://www.sqlbi.com/articles/from-sql-to-dax-projection/


#  recap

Recap:

1. Power Pivot
	- Model
		- 1.1.1. What are the dimension tables?
			- PK + Decs
		- 1.1.2. What are the Fact Tables?
			- FKs + Mesures
		- 1.1.3. Star Model,Snow Flake Model,Mixed Models
		- 1.1.4. Between two tables
			- a) Cardinality(1:1, \*:\*, \*:1, 1:\*)>> Default(\*:1)(Fact to Dim)
			- b) Cross Filter Direction (Single, Both) >> Default Cross Filter Direction is **Single**
			- c) Active/Inactive (This scenario of inactive relation comes if we have ROLE PLAYING DIMENSIONS)
	- DAX(Data Analysis eXpression)(Calculations)
		- 1.2.1. New Column(0.01%)
		- 1.2.2. New Mesure(99.98%)
		- 1.2.3. New Table(0.01%)
		- ![image](https://user-images.githubusercontent.com/20516321/148710242-8e059b9a-21e5-460f-b995-1f7c1689fdb3.png)

			- 1).Aggregation functions
				- SUM(Return value)
				- MIN
				- MAX
				- COUNT
				- COUNTA
				- SUMX
				- MINX
				- MAXX
				- COUNTX
				- COUNTAX
			- 2) Date and time functions
				- Calendar(\<start date\>,\<end date\>) (Returns Table)
				- CALENDARAUTO([\<end_of_the_fin_month\>](Return Table)
				- DATE (\<yyyy>,\<mm>,\<dd>)(Return Value)
				- DATEDIFF(\<startdate>,\<enddate>,\<interval>)(Return Value)
				- NOW()(Return Value)
				- today()(Return Value)
				- EOMONTH(\<DATE>,\<months>)(Return Value)

			- 3) Filter functions
				- Filter(\<Table>,\<filter>)(Return Table)
				- CalculateTable(\<Table>,\<filter>)(Return Table)
				- ALL([\<Table>,[<column]])(Return Table)
				- ALLEXCEPT(\<table>,\<column>[,\<column>[,…]])(Return Table)
				- Calculate(\<Expression>,[\<filter1>,[\<Filter2>...]])
				- SELECTEDVALUE())Returns slicer selected value/coresponding value
				
			- 4) Financial functions
			- 5) Information functions
				- HASONEVALUE(\<columnName>)(Return Value)(Bool)
				- ISBLANK(\<value>) 
				- USERNAME()
				- USERPRINCIPALNAME()
			- 6) Logical functions
				- AND
				- OR
				- IF
				- SWITCH
			- 7) Math and Trig functions
				- DIVIDE(\<num>,\<den>,[\<alternate Result>])
				- ABS
				- SIN(pi()/2)
				- COS(0)
				- SQRT(<number>)
			- 8) Other functions
				- BLANK()
				- ERROR()
			- 9) Parent and Child functions
				- PATH(\<empno>,\<mgrno>
				- ![image](https://user-images.githubusercontent.com/20516321/137073130-748c5efb-2208-4c6a-a4c5-effa23a3552a.png)

			- 10) RelationShip Functions
				- deptno10_data_only = FILTER(EMP,RELATED(DEPT[DNAME])="ACCOUNTING")

			- 11) Statistical functions
				- RankX

				
			- 12) Table manipulation functions
				- SUMMARIZEDCOLUMNS
				- ROLLUP
				- TOPN

## Questions:
----


1. Filter Vs Calculatedtable
2. calculate Vs Calculatetable
3. all vs allexcept
4. new column Vs New mesure
5. selectedvalue
6. sum Vs Sumx
7. summarize Vs Summarizecolumns
8. Calculatetable Vs Filter Vs Calculate
9. Hasonevalue

				
#  Power Pivot Modeling Lab


# `Power BI Desktop Modelling`
- It is also knon as **Power Pivot**
- In power pivot mainly we will do
    - Relation Ships(Among Queries)
    - DAX Formulas

## SCENARIO
VanArsdel is a company that manufactures and sells sporting goods. The company has offices in the United States (US) and several other countries. Its sales comprise of US sales and International sales. VanArsdel’s sales come from its owned manufactured products, as well as other manufacturers’ products.

You have successfully brought the US sales data from the Access database and the International sales data from a collection of CSV files to Power BI Desktop. 

Before you can start analyzing your data, you need to manage the table relationships within your data model and create new ones if necessary. To do so, you might need to create calculated columns or calculated tables for the relationships to be based on.
Once you have all the relationships created, you can create visualizations and start to analyze the data. However, you need to create additional measures to perform more advanced analysis with your data, which includes:

- Comparing current year YTD sales and last year YTD sales.
- Comparing sales of VanArsdel's manufactured goods to other manufacturers.


## LAB OVERVIEW

In this lab, you will create 
    - calculated columns 
    - calculated tables
    - create table relationships in your data model based on the calculated columns and tables you created. 
In addition, you will write several DAX expressions to create measures to be used to analyze VanArsdel’s sales data. Specifically, you will create the following measures:
1. `Total Sales:` calculates the total sales.
2. `LY Sales:` calculates last year sales.
3. `Sales Var:` calculates sales variance between this year and last year sales.
4. `Sales Var %:` calculates sales variance between this year and last year sales in percentage.
5. `YTD Sales:` calculates YTD sales.
6. `LY YTD Sales:` calculates last year YTD sales.
7. `YTD Sales Var:` calculates sales variance between this year and last year YTD sales.
8. `YTD Sales Var %:` calculates sales variance between this year and last year YTD sales in percentage.
9. `Total VanArsdel Sales:` calculates sales for VanArsdel manufactured goods.
10. `% Sales Market Share:` calculates the percentage of VanArsdel manufactured goods from the total sales.



## WHAT YOU’LL NEED
The “Lab 2 - Starting.pbix” file

## Exercise 1- Manage Table Relationships
Power BI Desktop has automatically detected and created table relationships. So the first step is to ensure all the relationships are properly created, and if not, create them yourselves.


1. Open the `Lab2 - Starting.pbix` file from our `Labdata/Lab2 folder`.
2. In the navigation pane on the left, click `Model`

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0000.png?raw=true).
    
3. Notice that there is a **many to one** relationship from the `ProductID` column on the `Sales` table to the `ProductID` column on the `Products` table.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0002.png?raw=true)
    
4. Notice that there is a **many to one** relationship from the `ManufacturerID` column on the `Products` table to the `ManufacturerID` column on the `Manufacturers` table.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0004.png?raw=true)

5. Drag the `Date` column on the `Sales` table to the `Date` column on the `Date` table.
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0003.png?raw=true)
    
6. Now you want to create a relationship between the `Sales` table and the `Locations` table. First, you merge the `Country` and `Zip` columns in both `Sales` and `Locations` table as a new column, `CountryZip`. Then, you create a relationship on the `CountryZip` column for both tables.
    - In the `navigation pane` on the left, click `Data`
    
        ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0005.png?raw=true).
        
    - In the navigation pane on the right, click `Location`.
    - On the Modeling ribbon, click New Column.
    - In the formula bar for the new column, type `CountryZip = Locations[Country] & ", " & Locations[Zip]`, and press `Enter`.
        
        ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0008.png?raw=true)
        
    - In the navigation pane on the right, click Sales.
    - On the Modeling ribbon, click New Column.
    - In the formula bar for the new column, type `CountryZip = Sales[Country Name] & ", " & Sales[Zip]`, and press `Enter`.
        
        ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0006.png?raw=true)
        
    - In the navigation pane on the left, click **Model**.
    - Drag the **CountryZip** column on the **Sales** table to the **CountryZip** column on the **Locations** table.
    
        ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0007.png?raw=true)
        
16. Click **Save**, to save the Power BI file.

## Exercise 2- Last Year Comparison

- You want to know how much sales (revenue) in total does the VanArsdel have and to compare this with the figure from the same period last year. You need to create several calculated measures to help with this comparison. To do so, in either the Report view or the Data view, right-click the Sales table, click New Measure, and type in the corresponding DAX formulas for the measure you want to create. This will create the measures with the Home Table properties set to the Sales table.
- Specifically, you will create the following measures:
    - `Total Sales:` calculates the total sales. Format this measure as Currency. (Hint: Check out the SUM function).
    - `LY Sales:` calculates last year sales. Format this measure as Currency. (Hint: You might find the CALCULATE and SAMEPERIODLASTYEAR function useful).
    - `Sales Var:` calculates sales variance between this year and last year sales. Format this measure as Currency. (Hint: This is simply the difference between Total Sales and LY Sales).
    - `Sales Var %:` calculates sales variance between this year and last year sales in percentage. Format this measure as Percentage. (Hint: This is simply the percentage of Sales Var from LY Sales. You might find the DIVIDE function useful).

1. In the navigation pane on the left, click `Data`
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0005.png?raw=true).
2. In the navigation pane on the right, click `Sales`.
3. On the Modeling ribbon, click `New Measure`.
4. In the formula bar for the new measure, type `Total Sales = SUM(Sales[Revenue])`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0009.png?raw=true)

5. On the `Modeling` ribbon, click `Format`, click `Currency`, and click `Currency general`.
6. On the Modeling ribbon, click New Measure.
7. In the formula bar for the new measure, type `LY Sales = CALCULATE([Total Sales],SAMEPERIODLASTYEAR(‘Date’[Date]))`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0010.png?raw=true)

8. On the `Modeling` ribbon, click `Format`, click `Currency`, and click `Currency general`.
9. On the `Modeling` ribbon, click `New Measure`.
10. In the formula bar for the new measure, type `Sales Var = [Total Sales] - [LY Sales]`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0011.png?raw=true)

11. On the `Modeling` ribbon, click `Format`, click `Currency`, and click `Currency general`.
12. On the `Modeling` ribbon, click `New Measure`.
13. In the formula bar for the `new measure`, type `Sales Var % = DIVIDE([Sales Var],[LY Sales]) `, and press `Enter`.

    
14. On the `Modeling` ribbon, click `Format`, and click `Percentage`.
15. Click `Save`, to save the Power BI file.
16. Develop below report and understand results

    ![image](https://user-images.githubusercontent.com/20516321/112080270-a8a33680-8ba7-11eb-8346-299e0f052cb2.png)


`Home Work:`
- Total Units: Total Units = SUM(Sales[Units])
- LY Total Units: LY Total Units = CALCULATE([Total Units],SAMEPERIODLASTYEAR(‘Date’[Date])
- Total Units Var: Total Units Var = [Total Units] - [LY Total Units]
- Total Units Var %: Total Units Var % = DIVIDE([Total Units Var],[LY Total Units])


## Exercise 3- Year to Date
- Year-to-date (YTD) is a period starting from the beginning of the current year and continuing up to the present date. You want to calculate the YTD sales and compare this with the figure from the same period last year. Specifically, you will create the following measures:
    - YTD Sales: calculates the YTD sales. Format this measure as Currency. (Hint: Check out the TOTALYTD function).
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0013.png?raw=true)
    
    - LY YTD Sales: calculates last year YTD sales. Format this measure as Currency. (Hint: You might find the CALCULATE and SAMEPERIODLASTYEAR function useful).
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0014.png?raw=true)
    
    - YTD Sales Var: calculates sales variance between this year and last year YTD sales. Format this measure as Currency. (Hint: This is simply the difference between YTD Sales and LY YTD Sales).
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0015.png?raw=true)
    
    - YTD Sales Var %: calculates sales variance between this year and last year YTD sales in percentage. Format this measure as Percentage. (Hint: This is simply the percentage of YTD Sales Var from LY YTD Sales. You might find the DIVIDE function useful).
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0017.png?raw=true)
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0110.png?raw=true)
    

`Home Work:`
1. YTD Total Units: YTD Total Units = TOTALYTD([Total Units],‘Date’[Date])
2. LY YTD Total Units: LY YTD Total Units = CALCULATE([YTD Total Units],SAMEPERIODLASTYEAR(‘Date’[Date]))
3. YTD Total Units Var: YTD Total Units Var = [YTD Total Units]- [LY YTD Total Units]
4. YTD Total Units Var %: YTD Total Units Var % = DIVIDE([YTD Total Units Var],[LY YTD Total Units])

## Exercise 4- Market Share

- VanArsdel sales comprise of products manufactured by VanArsdel and other companies. You want to know how much of these sales are VanArsdel’s own manufactured products. You decide to show this share in numbers and %. Specifically, you will create the following measures:
- Total VanArsdel Sales: calculates sales where the products manufacturer is VanArsdel. Format this measure as Currency. (Hint: Use the CALCULATE function and filter by Manufacturer).
- % Sales Market Share: calculates the percentage of sales of VanArsdel manufactured products from the total sales. Format this measure as Percentage.

1. In the navigation pane on the left, click `Data`.
2. In the navigation pane on the right, click `Sales`.
3. On the `Modeling` ribbon, click `New Measure`.
4. In the formula bar for the new measure, type `Total VanArsdel Sales = CALCULATE([Total Sales],Manufacturer[Manufacturer]="VanArsdel")`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0019.png?raw=true)

5. On the `Modeling` ribbon, click `New Measure`.
6. In the formula bar for the new measure, type `% Sales Market Share = IF([Total VanArsdel Sales]=0,0,DIVIDE([Total VanArsdel Sales],[Total Sales],0))`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0018.png?raw=true)

7. On the `Modeling` ribbon, click `Format`, and click `Percentage`.
8. Click `Save`, to save the Power BI file.

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0111.png?raw=true)

`Home Work:`
- Total VanArsdel Units: Total VanArsdel Units = CALCULATE([Total Units],Manufacturers[Manufacturer]=“VanArsdel”)
- % Units Market Share: % Units Market Share = IF([Total VanArsdel Units]=0,0,DIVIDE([Total VanArsdel Units],[Total Units],0))


## Exercise 5- Optimize the Data Model

1. Now that you have the table relationships defined and the measures created, you want to optimize the data model before you create the visualizations.
1. If it is not already open, open the Lab 2 - Starting.pbix file.
1. Ensure both the **International Sales** and **Country Population** table are hidden from the report view using the following steps.
1. In the navigation pane on the left, click `Data`.
1. In the navigation pane on the right, click the ellipses (...) adjacent to - `International Sales` and click `Hide in report view`.
1. In the navigation pane on the right, click the ellipses (...) adjacent to `Country Population` and click Hide in report view.
1. Hide the following fields on the `Date` table from the report view:
    - MonthNo
    - MonthID
    - Month
        - In the navigation pane on the right, click `Date`, click the ellipses (...) adjacent to `MonthNo` and click `Hide in report view`.
        - In the navigation pane on the right, click Date, click the ellipses(...) adjacent to `MonthID` and click `Hide in report view`.
        - In the navigation pane on the right, click Date, click the ellipses(...) adjacent to `Month` and click `Hide in report view`.
5. Sort the MonthName column by the MonthNo column using the following steps.
    - Click the `MonthName` column and, on the Modeling ribbon, click `Sort by Column`, and click `MonthNo`.
9. Hide the `CountryZip` field on the `Location` table and the `ManufacturerID` field on the `Manufacturer` table from the report view using the following steps.
    - In the navigation pane on the right, click Location, click the ellipses adjacent to CountryZip and click Hide in report view.
    - In the navigation pane on the right, click Manufacturer, click the ellipses adjacent to ManufacturerID and click Hide in report view.
10. Hide the following fields on the **Products** table from the report view.
    - ProductID
    - ManufacturerID
    - Manufacturer
        - In the navigation pane on the right, click Products, click the ellipses(...) adjacent to ProductID and click Hide in report view.
        - Click the ellipses adjacent to ManufacturerID and click Hide in report view.
        - Click the ellipses adjacent to Manufacturer and click Hide in report view.
8. Hide the following fields on the **Sales** table from the report view.
    - ProductID
    - Date
    - Zip
    - Units
    - Revenue
    - Country Name
    - CountryZip
        - In the navigation pane on the right, click Sales, 
        - Click the ellipses adjacent to `ProductID` and click `Hide in report view`.
        - Click the ellipses adjacent to `Date` and click `Hide in report view`.
        - Click the ellipses adjacent to `Zip` and click `Hide in report view`.
        - Click the ellipses adjacent to `Units` and click `Hide in report view`.
        - Click the ellipses adjacent to `Revenue` and click `Hide in report view`.
        - Click the ellipses adjacent to `Country Name` and click `Hide in report view`.
        - Click the ellipses adjacent to `CountryZip` and click `Hide in report view`.
9. Click `Save`, to save the Power BI file.

## Questions
----
1. Can you develop below report
    - ![image](https://user-images.githubusercontent.com/20516321/110577445-ac3ac480-8188-11eb-9afc-a39eb1443a41.png)


```python

```


```python

```

#  Exam

Exam 1:

https://docs.google.com/forms/u/2/d/1eHMES9qZATaOuvpYy3X2ewBDRm3flJt-CGFCahR6tac/edit


#  Power View Visualization Lab


# Power BI Desktop Visualization 

## Exercise 1- Cross-Tabular Report
- **Scenario:** You want to show VanArsdel's sales (revenue) and units for each month and year in a single report. You choose to show this using two Matrix visualizations.

1. Open file **Labdata/Lab3/Lab 3 - Starting.pbix** file.
1. In the navigation pane on the left, click **Report**.
1. In the **FIELDS** list, on the right, click the **Sales** table.
1. Drag the **Total Sales** field from the **Sales** table to the report to create a chart.
1. In the FIELDS list, on the right, click the **Date** table.
1. Drag the **MonthName** and **Year** fields from the **Date** table to the chart.
1. In the **VISUALIZATIONS** list, click **Matrix**.
1. In the **VISUALIZATIONS** list, in **Rows**, select **MonthName**, in **Columns**, select **Year**, and in **Values**, select **Total Sales**.
1. Click in the empty space of report
1. Repeat Step 3 to 8 to add another chart, but this time, display the **Total Units** field in place of **Total Sales**.
1. From the **Home** ribbon, click **Text** box.
1. In the text box, type **VanArsdel Sales and Units** and resize and move the text box so that it appears as the title of the report.
1. At the bottom of the screen, right-click **Page 1**, and click **Rename** Page.
1. Type **Sales and Units** and press **Enter**.
1. You should have something similar to the below Image:
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0023.png?raw=true)
1. Click **Save**, to save the Power BI file.    
### Think few mins, how to get below vizulization.

![image](https://user-images.githubusercontent.com/20516321/125020165-f9c33180-e095-11eb-9276-bf6689b976e9.png)

- Drag **Matrix** to work area
- Drag Year, Manufacturer, Region to **Rows**
- Drag **TotalSales** to **Values**
- Filter on **year** for **2001** and **2002**
- Filter on **region** for **Central** and **East**
- Filter on **Manufacturer** for **Abbas** and **Aliqui**
- Click **twice** on **Expand all down one level in the hierarchy**
- If you need **SubTotals** in the bottom set it in **format** tab

## Exercise 2- Part-to-Whole Report
**Scenario:** analyzing sales data by product category, segment and manufacturer.

1. Create a new report page by clicking **New Page (+)** at the bottom of the report view.
1. Drag the **Total Sales** field from the **Sales** table to the report and create a chart.
1. Drag the **Category** and **Segment** fields from the **Products** table to the chart.
1. In the **VISUALIZATIONS** list, click **100% Stacked Bar Chart** .
1. In the **VISUALIZATIONS** list, in **Axis**, select **Category**, in **Legend**, select **Segment**, and in **Value**, select **Total Sales**.
1. In the **VISUALIZATIONS** list, click the **Format** button.
1. Set **Data labels** to **On**.
1. Set **Value decimal places** to **0**.
1. Click on the empty space of report
1. Drag the **Total Sales** field from the **Sales** table to the report and create another chart.
1. Drag the **Manufacturer** field from the **Manufacturers** table to the chart.
1. Modify the chart to use the **Treemap visualization**.
1. Click on the empty space of report
1. Drag the **MonthName** field from the **Date** table to the report and create another chart.
1. Modify the chart to use the **Slicer visualization**.
1. Click on the empty space of report
1. Drag the **Year** field from the **Date** table to the report and create a chart.
1. Modify the chart to use the **Slicer visualization**.
1. Rename the report sheet to **Sales Breakdown**.
1. Click **Save**, to save the Power BI file.
1. You should have something similar to the below image:

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0024.png?raw=true)

## Edit Interactions:
Scenario: Slicer should not impact few vizulations.
- By Default Slicer changing all the visulizations inside the current page
- In above report click on year slicer > go to **Format** > click on **edit Interactions**  > select required vizulization **None** button.
- Now change any slicer options and observe the vizulation is not impacting.

## Sync Slicers
- In above report,copy any vizulaion and paste into other page .
- Go to view menu > click on **sync Slicers**
- select **year** slicer > select sync check boxes of current page and the pages need to impact.
- Change slicer options and observe that visulization changes.

## Exercise 3- Relationship Report

- **Scenario:** You would like to know more about the relationship between total units and total sales by category and segment. You choose to analyze this using scatter chart.

1. Create a new report page by clicking **New Page** at the bottom of the report view.
1. In **VISUALIZATIONS**, click **Scatter Chart**.
1. Drag the **Total Sales**, **Total Units**, and **YTD Sales** fields from the **Sales** table to the chart.
1. Drag the **Category** and **Segment** fields from the **Products** table to the chart.
1. Drag the **Year** field from the **Date** table to the chart.
1. Rename the report sheet to **Sales Relationship**.
1. Ensure that the following fields are set in the visualization Details:
    - Details: Category
    - Legend: Segment
    - X Axis: Total Sales
    - Y Axis: Total Units
    - Size: YTD Sales
    - Play Axis: Year
1. Click **Save**, to save the Power BI file.
1. You should have something similar to the below image:
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0025.png?raw=true)

## Exercise 4- Trend Report
**Scenario:** Show a chart to compare Total Sales and Total Units throughout the years. And then let's show two more charts showing the Total Sales and Total Units variances throughout the years.

1. Create a new report page by clicking the **New Page** icon at the bottom of the report view.
1. Drag the **Year** field from the **Date** table to the report and create the first chart.
1. Drag the **Total Sales** and **Total Units** fields from the **Sales** table to the Year chart.
1. Modify the chart to use the **Line and Stacked Column Chart** visualization.
1. Ensure that the **Year** is shown as the **Shared Axis**, **Total Sales** is shown as the **Column values**, and **Total Units** is shown as the **Line values** of the visualization Details.
----
1. Create a second chart based on the **Waterfall** Chart visualization.
1. Drag the **Sales Var** field from the **Sales** table to the Sales Var chart.
1. Drag the **Year** field from the **Date** table to the Sales Var chart.
---
1. Create a third chart, also based on the Waterfall Chart visualization.
1. Drag the **Total Units Var** field from the **Sales** table to the Total Units Var chart.
1. Drag the **Year** field from the **Date** table to the Total Units Var chart.
1. Click the Elipse button on both the Sales Var and Total Units Var charts and sort by **Year** ascending.
1. Add a **Text Box** to the report and enter **Yearly Trend** as the text.
1. Rename the report sheet to **Yearly Trend**.
1. Click **Save**, to save the Power BI file.
1. You should have something similar to the below image:

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0026.png?raw=true)

## Exercise 5- Rank Report
**Scenario:** You now want to analyze individual products sales (revenue) and volume (units). You decide to show these using two bar charts.

1. Create a new report page by clicking the **New Page** icon at the bottom of the report view.
1. Drag the **Total Sales** field from the **Sales** table to the report and create a chart.
1. Drag the **Product** field from the **Products** table to the chart.
1. Modify the chart to use the **Stacked Bar Chart** visualization.
1. Ensure that the chart is sorted by **Total Sales**.
----
1. Click on empty space of report
1. Drag the **Total Units** field from the **Sales** table to the report and create a new chart.
1. Drag the **Product** field from the **Products** table to the chart.
1. Modify the chart to use the **Stacked Bar Chart** visualization.
1. Ensure that the chart is sorted by **Total Units**.
-----
1. Click on empty space of report
1. Drag the **Year** field from the **Date** table to the report and create a new chart.
1. Modify the chart to use the **Slicer visualization**.
1. Modify the slicer type by clicking the **dropdown** arrow in the Year chart and selecting the **List** option.
1. Add a **Text Box** to the report and enter **Top Products** as the text.
1. Rename the report sheet to **Top Products**.
1. Click **Save**, to save the Power BI file.
1. You should have something similar to the below image:
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0027.png?raw=true)

## Reference

https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-report-visualizations

## Exercise 1:

![image](https://user-images.githubusercontent.com/20516321/115183931-64e61300-a0fa-11eb-9740-bc7eebf4f56a.png)

## Exercise 2:

https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-visualization-radial-gauge-charts

```python

```

#  Power View Hierarchy Drill down drill up


# Hierarchy

- Can you use **drill down/drill up** without **Hierarchy** ?
    - <input type="radio" disabled> Yes
    - <input type="radio" disabled checked> No
- Without Creating Hierarchy, can you drill down from **Category** to **segment** to **product**?   
    - <input type="radio"> Yes
    - <input type="radio" checked> No

## Exercise 1: Develop a report **Total Sales by Category**
- from fileds select total Sales and Category columns 
- select Stacked Column Chart
- Click on any bar to  move from category to segmant. Are you able to move ??? no right??? so let us learn how to create hierarchy

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0049.png?raw=true)

## Create Product Hierarchy

- In **Fields** Pane
- Expand **Product** table
- Select **Segment** and drag and drop on to **Category**
- Observe one hierarchy created with the name ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0050.png?raw=true)
- Rename **Category Hierarchy** as **Product Hierarchy**
- Select **product** Column and drop onto **Product Hierarchy**
- Finally your hierarchy will be looks like this

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0053.png?raw=true)



## Understanfd below terms and functionalties
    1. Drill Down
    2. Drill Up
    3. Show Next Level
    4. Expand Next Level
    
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0054.png?raw=true)

### Drill Down

    - Navigating from high level data to low level data (Example : Year > Half Year > Quarter > Month > Day)

1. In **Visulizations** > Click on **Stacked Column Chart**
1. From **Fields** pane > Click on **Total Sales** and **Product Hierarchy** 
1. Your report should look as shown below

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0055.png?raw=true)
    
1. **Click to turn on drill down** as shown below

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0056.png?raw=true)
1. Click on **Urban** bar and observe urban related **Segment** sales

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0057.png?raw=true)



### Drill Up

    - Navigating from low level data to high level data (Example : Day > Month > Quarter > Half Year > Year)
1. Click on **Drill Up** to see again **Category** Level Data

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0058.png?raw=true)

### Show Next Level
- Rolls data to next level irrespective of category

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0061.png?raw=true)

### Expand Next Level
- Shows category-Segment Data
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0062.png?raw=true)


```python

```

#  Power View Drill Through


# Drill Through

## Develop a Master Report
- In **Visulizations** > click on **Donut** Chart
- In **Fields** Pane > Click on **Category** and **Total Sales**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0063.png?raw=true)
    
- Rename page as **Master**
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0064.png?raw=true)


## Develop a Detail Report
1. In **Visulizations** > click on **Table** Chart
1. In **Fields** Pane > Click on **Category** , **Segment** and **Total Sales**
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0065.png?raw=true)
1. Select **Drill Through** and drag drop **Category**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0066.png?raw=true)
    
1. Rename page as **Detail**
1. Go Back to to **Master** page > Right Click on **urban** Category > Drill Through > Detail

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0068.png?raw=true)
1. Observe output of detail report

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0069.png?raw=true)


Refer: https://docs.microsoft.com/en-us/power-bi/desktop-drillthrough


```python

```

#  Types of Filter


# Filter data with Power BI
1. In PowerBI filters are mainly **6** types
    - Slicer
    - Filter Pane Filters
        - Vizulations Level Filter
        - Page Level Filter
        - All Pages Level Filter or Report Level Filter
    - Drill Through Filter
    - RLS(Row Level Security)

3. Data is the core of Power BI. As you explore reports, each visual draws its underlying data from sources that often contain far more data than you need. 
4. Power BI offers several ways to filter reports. Knowing how to filter data is the key to finding the right information
![](https://docs.microsoft.com/en-us/learn/modules/analyze-data-power-bi/media/2-1/power-bi-filter-intro.gif)

## Slicers
1. A simple type of filtering that you can use directly on the report page is called a slicer.
1. There are several different types of slicers: **numeric**, **categorical**, and **date**. 
1. Slicers make it easy to filter all the visuals on the page at once.

    ![](https://docs.microsoft.com/en-us/learn/modules/analyze-data-power-bi/media/2-1/power-bi-slicers.gif)
1.If you want to select more than one field, hold the Ctrl key and click additional fields.    

## Explore the Filters pane
1. Another way to filter data is by opening and modifying filters in the Filters pane. The Filters pane contains filters that were added to the report by the report designer. As a consumer, you can interact with the filters and save your changes but can't add new filters.

The **four types** of filters are:

1. **Filter on all pages** or **Report Level Filter** > Applies to all pages in the report.
1. **Filter on this Page** or **Page Level Filter** – Applies to all the visuals on the current report page.
1. **Visual level Filter** – Applies to a single visual on a report page. You only see visual level filters if you've selected a visual on the report canvas.
1. **Drillthrough Filter** – Allows you to explore successively more detailed views within a single visual.
    ![](https://docs.microsoft.com/en-us/learn/modules/analyze-data-power-bi/media/2-1/power-bi-filter-types.png)

### Filter on all pages or Report Level Filter
1. Open **Labdata/Lab3/Lab 3 - Starting.pbix**
1. Click on **New page** and rename it as **USA Region Wise Sales**
1. In **Visulizations**> Click on **Table**
1. From **Fields** > select **Country**,**Region** and **Total Sales**
1. Our report will be looks like below image

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0072.png?raw=true)
1. Right click on **USA Region Wise Sales** > Click on **Duplicate Page**
1. Rename page as **USA Region Wise Units**
1. Delete column **Total Sales** and drag **Total Units**
1. Drag and drop **Country** column below **Filter on all Pages** > Select **USA** > observe reports data in both the pages
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0073.png?raw=true)

### Filter on this Page or Page Level Filter
1. In above report **USA Region Wise Sales** > drag and drop **year** column onto **Filters on this page** > show only sales **greater than or equal** to **2006** and **less than or equal** to **2010**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0074.png?raw=true)
    
1. Observe report data

### Filter on this Visual
1. In above report **USA Region Wise Sales** > select **table visulization** > provide region filter as shown in below image 

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0075.png?raw=true)
    
1. Observe report data


### Drill Through
1. Refer previous lesson


### Reference
[Refer and complete learning path](https://docs.microsoft.com/en-us/learn/modules/analyze-data-power-bi/1-filtering-data)

### Questions:
1. How many Filters available in Power BI?

    - Slicer
    - Filter Pane
        - Viz
        - page
        - all pages
    - Drill Through
    - Row-Level Security(RLS)
2. What is the defualt sorting in slicer?
    - Ascending order
1.  Slicer by default will affect other pages visulizations? do you have any work arounds?
    - No, we have work arounds [Refer](https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-visualization-slicers#sync-and-use-slicers-on-other-pages) 
1.  I have a slicer and two visulas ,slicers need to affect only one visual,is it possible?
    - Yes. [Refer](https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-visualization-slicers#control-which-page-visuals-are-affected-by-slicers)
1. Can you create a slicer with two values "option1" and "option2"
    - Yes. create Custome table then create slicer using custom table [refer](https://docs.microsoft.com/en-us/power-bi/connect-data/desktop-enter-data-directly-into-desktop)
2. 
```python

```

#  Groups Bins


# Grouping and Binning

## Grouping
1. Open file **Labdata/Lab3/Lab 3 - Starting.pbix** file.
1. Expand **products** > Right click on **Segment** > Click on **New Group** > select as shown below

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0112.png?raw=true)

1. click on **pie chart**
1. drag **segment(groups)** into legend
1. drag **totalsales** into values
1. observe report

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0113.png?raw=true)


## Binning
1. Import **scott excel** file from **Labdata/Lab1**
1. Right click on sal column and develop as shown
    - Note: Default Number of bins are 5


    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0114.png?raw=true)
    
1. develop a report as shown

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0115.png?raw=true)

Reference: https://docs.microsoft.com/en-us/power-bi/desktop-grouping-and-binning


```python

```

#  Conditional Formatting


# Conditional Formatting

## Font Color Conditional Formatting

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0117.png?raw=true)


## Font Color Example 2
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0124.png?raw=true)



## Icons Condtional Formatting
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0123.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0121.png?raw=true)

https://docs.microsoft.com/en-us/power-bi/desktop-getting-started <br>
https://docs.microsoft.com/en-us/power-bi/desktop-conditional-table-formatting
## Ref

https://exceleratorbi.com.au/conditional-formatting-with-a-text-field-in-power-bi/


#  Power BI Service


# Power BI Service

## Create a new workspace

1. Signup for new user id and password with **work mail id** [Signup link](https://signup.microsoft.com/signup?sku=a403ebcc-fae0-4ca2-8c8c-7a907fd6c235&email=&ru=https%3A%2F%2Fapp.powerbi.com%3Fpbi_source%3Dweb_nolicense_redirect%26redirectedFromSignup%3D1%26noSignUpCheck%3D1) or **use what instructor provided to you**.
2. Open https://app.powerbi.com/
3. Signin with username and password given to you by your instructor
    ![image](https://user-images.githubusercontent.com/20516321/112792985-1658d200-9082-11eb-9f74-63b862b27d24.png)

4. In the left **Navigation Pane** > Click on **Workspaces** > Click on **Create a Workspace** > provide **workspace name** as **rritec-workspace** > click on **Save**

## Publish PBI Report

1. Open the **Labdata/Lab4/Lab 4 Starting.pbix** file.
1. On the **Home ribbon**, click **Publish**.
1. In Select a destination, select **rritec-workspace**, and click **Select**.
1. If prompted, sign in using the account you used to sign up for the Power BI service.
1. [Signup link](https://signup.microsoft.com/signup?sku=a403ebcc-fae0-4ca2-8c8c-7a907fd6c235&email=&ru=https%3A%2F%2Fapp.powerbi.com%3Fpbi_source%3Dweb_nolicense_redirect%26redirectedFromSignup%3D1%26noSignUpCheck%3D1)
1. Once the report is published, click Got it.
1. Open browser, go to https://app.powerbi.com/, and click Sign in.
1. Sign in using your account.
1. Go to the **Lab 4 Starting Report** and explore your published report. It looks similar to the one in Power BI Desktop file. Now you can start creating a dashboard by pinning some visualizations.
## Create Dashboard by Pining Visualizations
1. Go to the **Sales Report** tab and pin the chart showing **Total Sales by Category and Segment** (100% Stacked Bar Chart). Select to create a New dashboard and name it **VanArsdel Sales**.
1. Pin the **treemap chart**, **the scatter chart**, and the **map** visualization from the Sales Report tab to the **VanArsdel Sales** dashboard.
1. Go to the **Yearly Trend** tab and pin the **waterfall chart** that shows the **Sales Var by Year** to the VanArsdel Sales dashboard.
1. Go to the VanArsdel Sales dashboard and review what you have created.
1. Resize and arrange the tiles as necessary.
1. Go to **Edit** > Click on **Mobile Layout** > Observe how it looks in mobile > In the Right Side corner Click on **Web Layout** to see how it looks in web/laptops
1. Review the phone view.
1. Resize and arrange the tiles as necessary.
1. You should have something similar to the below image:

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0048.png?raw=true)
    
- **Note:** If the original visualization that's used to create the tile changes, the tile doesn't change. For example, if you pin a line chart from a report and then you change the line chart to a bar chart, the dashboard tile continues to show a line chart. The data refreshes, but the visualization type doesn't.

## Share Dashboard

1. Let's start sharing your newly created dashboard. For simplicity, let's share the dashboard to your own email address.

1. **NOTE:** Power BI Pro is required for sharing dashboards. If you do not have a Power BI Pro subscription, you can enroll for a free 60 day trial.

1. Click **My Workspace**, click Dashboards, and click **Van Arsdel Sales**.
1. In the **VanArsdel Sales** dashboard, click the **Share** button to share your dashboard.
1. Click **Try Pro** for free.
1. Click **Start Trial**, and click **Close**.
1. Click **My Workspace**, click **Dashboards**, and click **Van Arsdel Sales**.
1. In the **VanArsdel Sales dashboard**, click the **Share** button to share your dashboard.
1. In Grant access to, enter your email address used for Power BI service and click Share.
1. Check your inbox to see an invite to view this dashboard.

## Update Report and re-publish
----
1. Once you've published your Power BI Desktop file to Power BI service, you can still make changes to it, and re-publish the file so that your changes is reflected in Power BI service.
1. Open the **Lab 4 Starting.pbix** file.
1. Modify the **Total Sales by Category and Segment chart** (the one displayed using **100% stacked bar chart** visualization) on the Sales Report tab to use **Stacked Bar chart** visualization instead.
1. Again **publish** the file to **Power BI service** and replace the existing dataset with this one.
1. Go to Power BI service and review the **Lab 4 - Starting Report** and examine whether the change you made is reflected.

## Add entire page to dashboard as live page
1. Open report > click on **...** > Click on **Pin to a dashboard**
 
## Add Web Content Tile
----
4. Web Content Tile accepts any html tags/code
5. In above report click on **Edit** > Click on **+ Add tile**
6. Under Media, Clic on **Web Content**  > Select **Next** 
7. Under **Embed Code** > paste below code html

    ```
    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
    ```

1. Click om **Apply** and observe Tile in the dashboard

## Add Image Tile
-----

1. In above report click on **Edit** > Click on **+ Add tile**
1. Under Media, Clic on **Image**  > Select **Next** 
1. Under **Content** > paste below URL

    https://github.com/rritec/datahexa/blob/master/images/Mentor_dl.jpg?raw=true

1. Click om **Apply** and observe Tile in the dashboard    

## Add youtube Video
----

1. In above report click on **Edit** > Click on **+ Add tile**
1. Under Media, Clic on **Video**  > Select **Next** 
1. Under **Content** > paste below URL

    https://youtu.be/DNovBg5VCHA?list=PLpF-Cn8-Vi9QLt3NsK-7RH0jUPGRLnu7o

1. Click om **Apply** and observe Tile in the dashboard    

## Explore Dasboard Themes
----

#### Exercise 1: Export and import custom theme.

1. Open **PowerBI Desktop** > Open Any **report** > Go to **View** menu > Click on **Themes** down arrow mark > Click on **Customize Current Theme**
2. Observe all **properties**
3. Change required **colors** or **fonts** ...etc
4. Click on **Apply**
5. Again Go to **View** menu > Click on **Themes** down arrow mark > **Save Current Theme** into local pc **Desktop**
6. Open any other report > Go to **View** menu > Click on **Themes** down arrow mark > Click **Browse for themes** > Select previously saved **json** file > Click on **open** > observe changes

#### Exercise 2: Change Themes from Power BI Service.

1. In above report click on **Edit** > Click on **Dashboard Theme** > explore it

    - For more info [click here](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-report-themes)
  

## Questions
1. Without using **Power BI Desktop**, will you be able to upload **PBIX** file into **Power BI Service** ?
    - Yes. 
    - Go to required **workspace** > Click on **New** > Click on **Upload a File**
        ![image](https://user-images.githubusercontent.com/20516321/114537204-8e70eb80-9c6f-11eb-9c72-a4f0d0b68c5c.png)

  
  
#  Create Apps

## what is an App ?
- An app is a Power BI content type that combines related **dashboards and reports**, all in one place. An app can have one or more dashboards and one or more reports, all bundled together. 
- Click on **rritec-workspace** > click on **Create app** > name it as **rritec-workspace-app** > provide **description** as **it is a sales app**
- Click on **Publish app** > in pop up click on **publish**
- Explore [Here](https://docs.microsoft.com/en-us/learn/paths/manage-workspaces-datasets-power-bi/?ns-enrollment-type=Collection&ns-enrollment-id=djwu3eywpk4nm)

## Questions
1. If we created new report, will it automatically reflect into app?
  - No,We need to update the app
2. By default,a report or dashboard will be not shown in the app. Do we have any option to show a report or dashboard.?
  - Yes . (Go to workspace > view > list > Include in app > disable/enable it)
3. Can you create a report using published dataset? in side power bi service?
  - Yes
4. How Many Apps, possible using One Work Space ?
  - Only **One**
5. 


#  Parameters

# Parameters

- let us assume development servername and database name
    - Server name: rritec
    - Databasename: Adventureworksdw2012

- let us assume Testing servername and database name
    - Server name: rritec_test
    - Databasename: Adventureworksdw2012_test

- let us assume production servername and database name
    - Server name: rritec_prod
    - Databasename: Adventureworksdw2012_prod
- Import three tables DimDate,DimCustomer and FactInternetSales tables from sqlserver and observe M-Language source line of code of each query
- Create two paramatrs with the name of Servername and DBName and passvalues as rritec and AdventureWorksDW2012 respectively
    - ![image](https://user-images.githubusercontent.com/20516321/147030231-745ed8c7-e0a9-424b-bfa6-44e6d1e92647.png)
    - ![image](https://user-images.githubusercontent.com/20516321/147030273-c9c25483-2ef9-44a8-b6c4-a0ca1ddf82f0.png)


- Double click on each Query source step and change static values to above parameters.


## Reference M-Language
let
    Source = Sql.Database("rritec", "AdventureWorksDW2012"),
    dbo_DimDate = Source{[Schema="dbo",Item="DimDate"]}[Data]
in
    dbo_DimDate

let
    Source = Sql.Database("rritec", "AdventureWorksDW2012"),
    dbo_DimCustomer = Source{[Schema="dbo",Item="DimCustomer"]}[Data]
in
    dbo_DimCustomer

let
    Source = Sql.Database("rritec", "AdventureWorksDW2012"),
    dbo_FactInternetSales = Source{[Schema="dbo",Item="FactInternetSales"]}[Data],
    #"Filtered Rows" = Table.SelectRows(dbo_FactInternetSales, each [OrderDate] >= RangeStart and [OrderDate] <= RangeEnd)
in
    #"Filtered Rows"


#  Gateways Data Refresh in Power BI


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
8. 


#  Deployment Pipelines

## Power BI Deployment Pipelines
-----

- The tool is designed as a pipeline with three stages:

### Development

- This stage is used to design, build, and upload new content with fellow creators. This is the first stage in deployment pipelines.

### Test

- You're ready to enter the test stage after you've made all the needed changes to your content. You upload the modified content so it can be moved to this test stage. Here are three examples of what can be done in the test environment:
- Share content with testers and reviewers
- Load and run tests with larger volumes of data
- Test your app to see how it will look for your end users

### Production

- After testing the content, use the production stage to share the final version of your content with business users across the organization.

### Navigation Steps

1. Click on Workspace **rritec-workspace** > Click on **settings** > Click on Premium > select storage as small blobs > click on **ok**
1. Click on **Deployment Pipelines** > Click on **Create a Pipeline** > Provide pipeline name as **rritecPipeline** >click on **Assign Workspace** > from drop down select **rritec-workspace** > Select **Development** > Click on assign
1. Click on **Deploy** to copy content (Datasets/reports/dashboards) to **Test**
1. Click on Test **Deploy** to copy content from **Test** to **production**
### On going Changes:
1. How to deploy new 1 or couple of reports into other environment?
2. How to deploy Modified report from lower environment to higher environment?
3. How to decommission(Delete) a report?
### Questions
1. After deployment(from dev to test) one report added to dev. Then will it automatically will appear in test?
  - NO, We need click on Dev **Deploy** button
2. As a developer what workspace i will have access?
  - Dev
3. Accidentely removed one report from Dev, Can i copy a report from test to dev?
  - No. (Work around is Request Admin to download PBIX file from test and publis pbix file to Dev)
4. 


#  Bookmarks Actions Buttons Images



# Reading Activity:
https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-bookmarks

https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-buttons


## Use Case 1: Clear All Slicers in Power BI
----
1. Create a **text box** and name it as Dname:
1. Create a **Slicer** with Dname Column
1. Create a **text box** and name it as Job:
1. Create a **Slicer** with Job Column
1. Develop a pie chart location by salary 
1. Develop a pie chart Ename by salary 
1. Kepp two slicers with all option
1. Go to view menu create a book mark and rename it has **Clear All**
1. Create a **Blank** Button > Select it change **Button Text** as **Clear All** > Select **action** as **Clear All** book mark
1. Change slicers as you wish  and observe data
1. press ctrl and click on button it will reset all slicers to **all**

![image](https://user-images.githubusercontent.com/20516321/209264366-34062b18-eeb1-4b6f-a76c-47e16aab8464.png)

## Use Case 2: Toggle between Pie and Bar Chart
----
1. Open Power BI Desktop
2. Import DimCustomer.csv and FactInternetSale.csv
3. Develop a pie chart and column chart one overap another
4. Change titles of visulizations as Pie and Bar respectively
5. Open Selection pane and Bookmarks pane
6. Hide Column chart and create bookmark as Pie
7. Hide Pie chart and create bookmark as Column
8. From google download two images Pie and bar chart
9. Go to insert menu and click on images and browse above pie and place in the work area as small as possible
10. Go to insert menu and click on images and browse above bar and place in the work area as small as possible
11. Select Pie image > enable Actions > select bookmarks as pie
12. Select Bar image > enable Actions > select bookmarks as Bar
13. Test it

![image](https://user-images.githubusercontent.com/20516321/113813419-7b50ae00-978d-11eb-9718-acd2f1cc6c79.png)

## Use Case 3: Navigate to required page of PBIX file Dynamically
----

- Create custom table by using Enter Table option
    - In **Power BI Desktop** > Click on **Enter Data** > Provide **Table Name**, **Column Name** and Values must be equal to your PBIX page names 
    - For Example
        ![image](https://user-images.githubusercontent.com/20516321/116339897-e117df00-a7fb-11eb-95eb-517087b67597.png)
- Develop a slicer using above column and make it as single selection
- Introduce one Image and allign beside slicer as shown below image
- select Image > Go to format > action > Type: **Page Navigation** > Destination: Click on **Fx** > Format By: **Field Value** > Based on Field: **Select column what you created** > Click on **ok**


![image](https://user-images.githubusercontent.com/20516321/113814794-d1beec00-978f-11eb-9e36-7511da5f7002.png)


1. **Reference**
    https://radacad.com/clear-all-slicers-in-power-bi-a-bookmark-story
    
    https://radacad.com/bookmarks-and-buttons-making-power-bi-charts-even-more-interactive
    

#  Power BI Import Vs Direct Query Vs Live Connection


https://docs.microsoft.com/en-us/power-bi/power-bi-data-sources

Example:

Excel has no direct Query

Sql Server has Direct query

![image](https://user-images.githubusercontent.com/20516321/113528602-a779fc80-95de-11eb-938a-3808cc990206.png)


![image](https://user-images.githubusercontent.com/20516321/113528740-1d7e6380-95df-11eb-9d46-946971a3287a.png)


https://radacad.com/directquery-live-connection-or-import-data-tough-decision
https://docs.microsoft.com/en-us/power-bi/connect-data/desktop-directquery-about

	Import(90%)	Direct Query/Live Connection(10%)	Comments
Memory(Hard Disk Space)	(metadata + Data)2044KB	(Metadata)32KB	"1. Publish Limitation of PBIX file is 1GB
2. PBIS Storage follows Column-store in-memory technology"
Performance	High Speed	Low Speed	
Features	All Dax Functions using possible	Few Dax Functions using possible	
![image](https://user-images.githubusercontent.com/20516321/183326168-df918024-1b3e-42c1-aa85-b0a2042cf906.png)


## Questions
---
1. How many types of connection available in Power BI
  - Import
  - Direct Query
  - Live Connection
  - Stream
2. What is the size limit of dataset in power BI Service Pro ?
  - 1GB
3. For Each Power BI Service, what is the total size limit of datasets?
  - 10 GB
4. Data inside PBIX file stores in what format?
  - Columnar Store
  - Compresed format(Due to this Size will be reduced to approximately below 10% actual size)
  
5. Import Data Connection Pros and Cons
  - Pros
    - Power BI Fully Functional
      - we can use time intilligency functions
      - Query combineing
      - ...etc
    - Performance is very good as data already available inside poer bi service
    - it is possible with all data sources(file/Databases/web/...etc)
  - Cons
    - Size limitations
    - Shedule data sets by following ETL data refresh window
  
6. Direct Query/Live Connection Connection Pros and Cons
  - Pros
    - No need of schudling dataset always we will get latest data from database
    - No Hard disk space or power Bi service space consumed
  - Cons
    - Can not support all data sources
    - Performance is not good as it as to run query in the runtime and fetch results from database
    - Power BI all fetures are not supported
7. Always give first priority to Import connection
8. Live connection available only for SSAS Tabular Models and SSAS Multidimensional Cubes
9. Can you swtich Import Connection of table to Direct Query?
  - No
10. Can you swtich Direct Query Connection of table to Import?
  - Yes
 11. What is Dual Storage, when we will use it.
  - https://docs.microsoft.com/en-in/power-bi/transform-model/desktop-storage-mode


```python

```

#  Run Python scripts in Power BI Desktop


# Run Python scripts in Power BI Desktop

    


1. Follow this blog
    https://docs.microsoft.com/en-us/power-bi/desktop-python-scripts


**If time permits listen below videos**



1. Listen videos to learn basics of python https://datahexa.com/course/python-basic-level-1/

1. Set up new python environment by listening below video

    [![IMAGE ALT TEXT HERE](http://img.youtube.com/vi/HWo1dJTpwOc/0.jpg)](http://www.youtube.com/watch?v=HWo1dJTpwOc)

```python

```

#  SSAS Multidimensional Models in PowerBI Desktop


# SSAS Multidimensional Models(Cubes)

## MSBI

    - SSIS > ETL
    - SSRS > Reporting
    - SSAS > Tabular Cube or Multidimensional Cube

## Download and Restore Sample Data

1. Download Sample Data warehouse data **AdventureWorksDW2012.bak**

    https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorksDW2012.bak

1. Restore Data by following below steps

    https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15#restore-backup

## Install SQL Server Analysis Services
1. Start > Microsoft SQL Server 2019 > SQL Server 2019 Installation Center (64-bit)
1. Click on Installation > New Sql Server Stand alone installation or add Features to existing installation> select c drive > sql2019 folder > Developer_enu
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0139.png?raw=true)
1.  Select Add fetures to an existing instance
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0140.png?raw=true)
1. Select Analysis Service
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0141.png?raw=true)
1. Follow the wizard    



## Learn Basic of SSAS
1. Setup prerequisites

    https://docs.microsoft.com/en-us/analysis-services/multidimensional-tutorial/multidimensional-modeling-adventure-works-tutorial?view=asallproducts-allversions#prerequisites

1. Complete at least first 2 chapters 

    https://docs.microsoft.com/en-us/analysis-services/multidimensional-tutorial/multidimensional-modeling-adventure-works-tutorial?view=asallproducts-allversions

## Deploy Cube
1. Open **SQL Server Data Tools for Visual Studio 2012** > **File** > **Open** > **Project/Solution** > **Lesson 10 Complete** > select **Analysis Services Tutorial.sln** > Click on **open**
1. In **Solution Explorer** > Right click on **Analysis Services Tutorial** > Click on **Deploy**

## Develop PBI Report using Cube
1. Open **PBI Desktop** > **Get Data**> **SQL Server Analysis Service Database**
1. Provide **Server** as **localhost** > Select **Connect Live** > Click on **ok**
1. Expand **Analysis Service Tutorial** > Select **Sales Summary** > Click on **ok**
1. Select **Calendar Date** Hierarchy and **Total Sales Amount**
1. Observe Report
1. Similarly Develop some other reports


## Optional
- Lear SSIS by using MSFT documents
    - https://docs.microsoft.com/en-us/sql/integration-services/lesson-1-create-a-project-and-basic-package-with-ssis?view=sql-server-ver15-  
- SSRS
    - https://docs.microsoft.com/en-us/sql/reporting-services/install-windows/install-reporting-services?view=sql-server-ver15
    - https://docs.microsoft.com/en-us/sql/reporting-services/reporting-services-tutorials-ssrs?view=sql-server-ver15



```python

```

#  Connect to a Snowflake computing warehouse in Power BI Desktop


1. Create **Snowflake** data warehouse
    1. Sign up for free account
	- Click [here](https://signup.snowflake.com/?_ga=2.244222469.1468146556.1618626004-173092964.1618626004) and create id 
	- Provide all information like name and mailid  > click **Continue** > Choose your Snowflake edition as **Enterprise** > Choose your cloud provider as **Microsoft Azure** > Region as **West US2 (washington)** > click on **Get Started** > Open Mail > Verify mail to activate the account > create username and password
	![image](https://user-images.githubusercontent.com/20516321/115165273-bd052100-a0ca-11eb-89f9-a2443e23c786.png)

	- 
    
  
1. Open PBI Desktop
1. Connect snowflake
		1. Server > xxxxxxxx.west-us-2.azure.snowflakecomputing.com
		2. Warehouse > COMPUTE_WH > click on **ok**
		3. provide username: xxxxxx  > pasword: xxxxxx > click on **connect**
		
1. Select Required Table

	1. Expand Snowflake_sample_data > expand TPCH_SF1 > select tables Customer,Nation,Region,Orders
	1. Create joins accordingly.

    
1. Develop the report using columns region name ,nation name and total price.

    

**Optional:**

  1. Install snowsql CLI https://sfc-repo.snowflakecomputing.com/snowsql/bootstrap/1.2/index.html
  1. https://docs.snowflake.com/en/user-guide/getting-started-tutorial.html#snowflake-in-20-minutes
  
**Scripts:**
```
account_name: ox16000.west-us-2.azure
account url : https://ox16000.west-us-2.azure.snowflakecomputing.com
sername: kumaryama
password: ********



open cmd
snowsql -a uk00084.west-us-2.azure -u mylageethika
create or replace database sf_tuts;
select current_database(), current_schema();
create or replace table emp_basic (
  first_name string ,
  last_name string ,
  email string ,
  streetaddress string ,
  city string ,
  start_date date
  );
  
  
create or replace warehouse sf_tuts_wh with
  warehouse_size='X-SMALL'
  auto_suspend = 180
  auto_resume = true
  initially_suspended=true;
  
select current_warehouse();

put file://c:\temp\employees0*.csv @sf_tuts.public.%emp_basic;

list @sf_tuts.public.%emp_basic;
copy into emp_basic
  from @%emp_basic
  file_format = (type = csv field_optionally_enclosed_by='"')
  pattern = '.*employees0[1-5].csv.gz'
  on_error = 'skip_file';
select * from emp_basic;
insert into emp_basic values
  ('Clementine','Adamou','cadamou@sf_tuts.com','10510 Sachs Road','Klenak','2017-9-22') ,
  ('Marlowe','De Anesy','madamouc@sf_tuts.co.uk','36768 Northfield Plaza','Fangshan','2017-1-26');
select email from emp_basic where email like '%.uk';
select first_name, last_name, dateadd('day',90,start_date) from emp_basic where start_date <= '2017-01-01';

drop database if exists sf_tuts;

drop warehouse if exists sf_tuts_wh;

!exit

```

#  row level security (RLS)


# Security
In any BI application 3 Tiers of Security required. Those are
1. Authentication
  - Application username and password is called as Authentication.
2. Autherization
  - Object Level (Workspace, App,Dashboard,Report,Dataset)
    - https://docs.microsoft.com/en-us/power-bi/collaborate-share/service-new-workspaces
    - https://docs.microsoft.com/en-us/power-bi/collaborate-share/service-roles-new-workspaces
  - Row Level Security(RLS) or Data Security 
# Row Level Security (RLS)

## Reference Documents

https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-rls



## Develop Data Security in Dynamic Way

1. Copy below data into Excel

| Item      | Price | Account Manager     |
| ---        |    ----   |          --- |
| Item 1      | 10       | studentpbi@mylaramreddy.onmicrosoft.com   |
| Item 2   | 20        | studentpbi@mylaramreddy.onmicrosoft.com      |
| Item 3   | 30        | vmyla1@mylaramreddy.onmicrosoft.com      |
| Item 4   | 40        | vmyla1@mylaramreddy.onmicrosoft.com      |

2. Save the excel as rritec_rls_source
3. Import the excel and develop a table report with three columns
![image](https://user-images.githubusercontent.com/20516321/114550670-15c65b00-9c80-11eb-8129-9e0bef38f3a4.png)

4. Click on the model > Click on the Manage Roles > Create a role as shown below
![image](https://user-images.githubusercontent.com/20516321/114550922-5d4ce700-9c80-11eb-91eb-afe79589603c.png)

5. Save this report as rls_report
6. Publish to workspace.
7. In the workspace make sure **info@datahexa.com** as **Viewer**
8. Go to Dataset > Security > Select **role** and map info@datahexa.com > Add > Save 
9. Open **Private window** in the brwoser > open app.powerbi.com > login using info@datahexa.com and password shared by your instructor.
10. Open the report and notice that only two records are visible
![image](https://user-images.githubusercontent.com/20516321/114551387-f24fe000-9c80-11eb-8dcd-0bfd582b64a4.png)



## Questions
1. RLS will applies to Workspace members assigned Admin, Member, or Contributor ?
  - No . Only applies on Viewers
2. 
```python

```

#  Power BI Cmdlets for Windows PowerShell and PowerShell Core

## Reading Activity

- https://docs.microsoft.com/en-us/learn/modules/introduction-to-powershell/

# Power BI Cmdlets for Windows PowerShell and PowerShell Core
https://docs.microsoft.com/en-us/powershell/power-bi/overview?view=powerbi-ps

## Exercise 1: Install all modules of PowerBI
-----
1. Open **Windows PowerShell ISE(X86)** > In power Shell window run below command
```
Install-Module -Name MicrosoftPowerBIMgmt
```
2. In right side **Commands** window click on refresh observe all **six** useful modules are installed.
```

MicrosoftPowerBIMgmt.Admin
MicrosoftPowerBIMgmt.Capacities
MicrosoftPowerBIMgmt.Data
MicrosoftPowerBIMgmt.Profile
MicrosoftPowerBIMgmt.Reports
MicrosoftPowerBIMgmt.Workspaces
```
## Exercise 2: Export workspaces/Dashboards/Reports to csv file
-----

1. Click on **New Script** > paste below code and change **workspace id** and **path** accordingly and run it
```
Connect-PowerBIServiceAccount


Get-PowerBIWorkspace | Export-Csv -Path C:\Users\ramreddymyla\Desktop\rritec\20210731\cmdlets\ws.csv
Get-PowerBIDashboard -WorkspaceId 987a132d-795b-406e-9358-b6fbd3fade8f | Export-Csv -Path C:\Users\ramreddymyla\Desktop\rritec\20210731\cmdlets\ds.csv
Get-PowerBIReport -WorkspaceId 987a132d-795b-406e-9358-b6fbd3fade8f | Export-Csv -Path C:\Users\ramreddymyla\Desktop\rritec\20210731\cmdlets\rs.csv
```

## Exercise 3: Get report names from multiple workspaces

   
    $myArray = "9c265642-a2b2-4ae1-a7fe-d9f3822984d7","1083fdff-a6fd-4a92-b849-4387530e8a38"
    #$myArray.Length-1
    $i=0
    for(;$i -le $myArray.Length-1;$i++)
    {
        $myArray[$i]
        Get-PowerBIReport -WorkspaceId $myArray[$i] | Export-Csv -Append -Path C:\work\ps\list_of_sanjay_ws_reports1.csv
    }
    
   
            
### Exercise 4: Get report names from all workspaces

    
      # connect to power BI Service
      Connect-PowerBIServiceAccount


      # Define variables for path and file name
      $path="C:\work\ps\"
      $ws_file_name="list_of_workspaces.csv"
      $rs_file_name="list_of_reports.csv"

      # Export all workspace information
      Get-PowerBIWorkspace | Export-Csv -Path $path$ws_file_name

      # Read csv file of workspaces
      $ws=Import-Csv -Path $path$ws_file_name

      # Read ids of workspaces
      ForEach-Object {
          $Ids += $ws.Id
      }

      # export reportnames from each workspace in append mode

      $i=0
      for(;$i -le $Ids.Length-1;$i++)
      {

          Get-PowerBIReport -WorkspaceId $Ids[$i] | Export-Csv -Append -Path $path$rs_file_name
      }
    
   

## Exercise 5: Create new workspace
-----
```
New-PowerBIWorkspace -Name myla1-workspace
```

## Exercise 6: Remove Power BI Report
----
1. Change report id and workspace id and run it.

```
Remove-PowerBIReport -Id 09d39a15-65ac-46c8-84ac-de2923536cb9 -WorkspaceId 383e66d4-0587-45c8-93dd-0b4a8abec074
```

## Exercise 7: Add/Remove user to/from workspace
----

```
Add-PowerBIWorkspaceUser -Id 79578b7e-3515-421b-bb3f-1fbaee65a319 -UserEmailAddress info@datahexa.com -AccessRight Viewer
Remove-PowerBIWorkspaceUser -Id b901218c-3621-4238-883d-1a7abfdcb58b -UserPrincipalName info@datahexa.com
```
## Exercise 8: Bulk users adding to required workspaces
-----
- Download sample securiy [file](https://github.com/rritec/powerbi/blob/master/Labdata/setup-powerbi-access-to-end-users1.csv) 

      # Define variables for path and file name
      $path="C:\work\ps\"
      $file_name="setup-powerbi-access-to-end-users1.csv"


      # Read csv file of workspaces
      $ws=Import-Csv -Path $path$file_name
      #$ws
      #$Id1=""
      #$UserEmailAddress=""
      #$AccessRights=""

      #Clear-Variable wsId
      #Clear-Variable UserEmailAddress1
      #Clear-Variable AccessRights1

      # Read ids of workspaces
      ForEach-Object {
          $wsId += $ws.workspaceid
          $UserEmailAddress1 += $ws.UserEmailAddress
          $AccessRights1 += $ws.AccessRight   

      }

      # export reportnames from each workspace in append mode

      $i=0
      for(;$i -le $wsId.Length-1;$i++)
      {

          Add-PowerBIWorkspaceUser -Id $wsId[$i] -UserEmailAddress $UserEmailAddress1[$i] -AccessRight $AccessRights1[$i]



      }
      Clear-Variable wsId
      Clear-Variable UserEmailAddress1
      Clear-Variable AccessRights1
## Exercise 9: Disconnect Power BI Service
----

```
Disconnect-PowerBIServiceAccount
```

#  Paginated Reports

# Install Report Builder Tool

#  SSRS

Step 1: Install data tools
https://github.com/rritec/powerbi/blob/master/Notebooks/PBI_01_01_Introduction_Installation.md#instal-msbi-download-sql-server-data-tools-ssdt
Step 2: Follow the Tutorial
https://docs.microsoft.com/en-us/sql/reporting-services/create-a-basic-table-report-ssrs-tutorial?view=sql-server-ver15


#  Migrate SSRS to PowerBI

https://docs.microsoft.com/en-us/power-bi/guidance/migrate-ssrs-reports-to-power-bi


#  Power BI Interview Questions

1. Tell me about your self
   1. I completed [Btech] in [cse] specilaization and got opprtunity to work as fresher in [abc] company. I got onboard/Induction training on skills SQL and               PowerBI.
   2. From last 3 years iam working as a power Bi developer.
   3. In current Project iam working in IC role. As part of this role i will be speaking directly with Product Owner and getting user stories in jira board. We are         following 4 standard user stories 1) Requirment Gathering 2) Development 3) Testing 4) Deployment
   4. In current Project Iam working with Pobwer BI and SQl are main skills.
   5. In Power BI the building blocks which iam working are power Query, Power Pivot, Power View, and Power BI Pro and Premium license
	
2. **What are the important components of Power BI?**

    Important components of Power BI are: 
    1. Power BI Desktop
        1. Power Query Editor
        2. Power Pivot
        3. Power View
    2. Power BI Service
    3. Power BI Mobile
3. **What you know about Data Analysis Expressions (DAX)**

     Data Analysis Expressions (DAX) is a library of functions and operators that can be combined to build formulas and expressions in

        1. Power BI Desktop
        2. Azure Analysis Services
        3. SQL Server Analysis Services
        4. Power Pivot in Excel data models.

     DAX formulas include functions, operators, and values to perform advanced calculations and queries on data in related tables and columns in tabular data models    
4. **Data types of DAX?**
    1. Whole Number
    2. Decimal Number
    3. Boolean
    4. Text
    5. Date
    6. Currency
    refer more details [here](https://docs.microsoft.com/en-us/dax/dax-overview#data-types)
5. **Name two types of connectivity modes in Power BI?**
      1. Import
      2. Direct Query
6. Explain DAX Function Crossfilter
	1. [Read it](https://docs.microsoft.com/en-us/dax/crossfilter-function#:~:text=There%20are%20two%20ways%20to,work%20for%20just%20this%20measure.)
7. How to keep images in Slicer? and filter visulizations based on image selection?
8. How to show negative Values in pie chart?
9. What is HASONEVALUE DAX formula ? Develop Some report?
   1. https://docs.microsoft.com/en-us/dax/hasonevalue-function-dax
10. How to use **selectedvalue**
    1. https://docs.microsoft.com/en-us/dax/selectedvalue-function
11. what is ALL dax formula?
12. How to use particulat direction in one mesure calculation?
13. How to implement RLS?
14. How to use Mesure in slicer?

15. How to pass multiple values of disconnected table to visulization?

16. Difference between sum vs sumx in dax.

    1. https://radacad.com/sum-vs-sumx-what-is-the-difference-of-the-two-dax-functions-in-power-bi

17. common table expression in sql server example
18. Create table from view in sql server?

19. What is query folding in power bi
    1. https://docs.microsoft.com/en-us/power-query/power-query-folding
20. How to add images ?
    1. https://www.blue-granite.com/blog/simple-steps-to-embed-images-in-power-bi
21. Count Vs CountA 
22. Rolling Months
    1. https://stackoverflow.com/questions/49146565/show-last-3-months-from-selected-month-in-power-bi
    2. https://www.youtube.com/watch?v=duMSovyosXE

23. Number of unique rows – by multiple columns
    1. https://exceltown.com/en/tutorials/power-bi/powerbi-com-and-power-bi-desktop/dax-query-language-for-power-bi-and-power-pivot/number-of-unique-rows-by-multiple-columns/
	
24. Can you  do sub totals in table visulization?
    1. https://docs.microsoft.com/en-us/power-bi/visuals/desktop-matrix-visual#subtotals-and-grand-totals-with-matrix-visuals

25. What is stepped-layout-with-matrix-visuals
    1. https://docs.microsoft.com/en-us/power-bi/visuals/desktop-matrix-visual#stepped-layout-with-matrix-visuals
	
26. How Many Built-in Joins available in Power BI?


	   1. Inner Join 
	   2. Left Outer Join
	   3. Right Outer Join
	   4. Full Outer Join
	   5. Left Anti Join
	   6. Right Anti Join


27. See all these 

    1. https://data-flair.training/blogs/power-bi-interview-questions/
    2. https://data-flair.training/blogs/power-bi-interview-questions-and-answers/

28. Think and develop below reports.
	![image](https://user-images.githubusercontent.com/20516321/115226802-44837c00-a12d-11eb-94d3-b1ced898ddf1.png)
	![image](https://user-images.githubusercontent.com/20516321/115226863-57964c00-a12d-11eb-8d66-f248102aa75a.png)



29. Think and develop below reports.
	![image](https://user-images.githubusercontent.com/20516321/115226962-785ea180-a12d-11eb-991c-623b1c43dccd.png)
	![image](https://user-images.githubusercontent.com/20516321/115227020-8ca29e80-a12d-11eb-83e2-ca85877e5bca.png)


30. Do you know Power BI Rest API?
31. Do you know power Shell commands of Power BI?
	- https://docs.microsoft.com/en-us/powershell/power-bi/overview?view=powerbi-ps
	- Right click on  Windows power shell ISE > Run as Administartor 
	- Install all below moduls
		```
		Install-Module -Name MicrosoftPowerBIMgmt
		Install-Module -Name MicrosoftPowerBIMgmt.Admin
		Install-Module -Name MicrosoftPowerBIMgmt.Capacities
		Install-Module -Name MicrosoftPowerBIMgmt.Data
		Install-Module -Name MicrosoftPowerBIMgmt.Profile
		Install-Module -Name MicrosoftPowerBIMgmt.Reports
		Install-Module -Name MicrosoftPowerBIMgmt.Workspaces
		```
	- In Power Shell > Click on **New Script** > copy paste below code and change path accordingly.
		```
		Connect-PowerBIServiceAccount
		Get-PowerBIWorkspace | Export-Csv -Path C:\work\powerbi-powershell\ws.csv
		Disconnect-PowerBIServiceAccount
		```
	Click on Run > observe Csv file output
32. Project Methodology (Agil)
33. Errors rectifing (debugging)
34. What is the definition of L1, L2, L3, L4 support levels in IT Operations Management?
	- https://myfirstsite99.wordpress.com/what-is-the-definition-of-l1-l2-l3-l4-support-levels-in-it-operations-management/
35. Write Sql Query to get running totals.
	```sql
	select empno,sal,
	sum(sal)over (order by empno) 
	from emp
	order by empno
	```
36. Difference between summarize and summarizecolumns
    * https://www.sqlbi.com/articles/introducing-summarizecolumns/#:~:text=Another%20difference%20between%20SUMMARIZE%20and,only%20and%20no%20row%20context.
37. Explain about data alerts ?
    https://docs.microsoft.com/en-us/power-bi/create-reports/service-set-data-alerts
38. How many types of gateways are available in power BI?
    1. Personal Gateway
    2. Enterprise gateway
39. When we need to gateway?
    1. For on permise data sources(for example Oracle,Sql Server ,MySql,Excel, Notepad ...etc)
40. What are the ticketing tools available ?
    1. Ivanti
    2. Zendesk
    3. Freshservice ....etc
41. What is GetData in PowerBI ?
    1. GetData is a simple icon on PowerBI used to import data from the source.
42. List out some drawbacks/limitations of using PowerBI ?
    1. PowerBi Doesn't accepts file sizes larger than 1GB and doesn't mix imported data accessed from real-time connections.
    2. There are very few data soures that allow real-time connections to PowerBi reports and dashboards.
    3. it only shares dashboards and reports with users logged in with the same email address.
    4. Dashboard doesn't accept or pass user,account,or other entity parameters.
43. Name some commonly used tasks in the query editor ?
    1. Connect to data
    2. Shape and Combine data
    3. Group rows
    4. Pivot columns 
    5. Create custom columns 
    6. Query formulas
44. How many types of buildings blocks in power BI ?
    There are Five Types of Building Blocks
    1. Visualizations
    2. Datasets
    3. Reports
    4. Dashboards
    5. Tiles
45. What is Visualizations ?
    * Visualization is the visual representation of data in the form of maps, charts, or tables.
46. What is Datasets ?
    * Dataset is a collection of data gathered from various sources like SQL Server, Azure, Text, Oracle, XML, JSON, and many more. With the GetData feature in Power       BI, we can easily fetch data from any data source.
47. What is Report ?
    * Reports are a structured representation of datasets that consists of multiple pages. Reports help to extract important information and insights from datasets         to take major business decisions.
48. What is Dashboard ?
    * A dashboard is a single-page representation of reports made of various datasets. Each element is termed a tile. 
49. What is Tile ?
    * Tiles are single-block containing visualizations of a report. Tiles help to differentiate each report 
50. Name any 3 most useful aggregation functions DAX?
    DAX has a number of aggregation functions, including the following commonly used functions:
        * SUM
        * AVERAGE
        * MIN
        * MAX
        * SUMX (and other X functions)

51. Name any 3 most useful text functions in DAX?
    The text functions in DAX include the following:
       * CONCATENTATE
       * REPLACE
       * SEARCH
       * UPPER
       * FIXED

52. What are formats in Power BI ?
    1. Power BI Desktop – Power BI Desktop can be downloaded and installed on your PC. You can connect it to the data source, transform the data, and analyze and             visualize it with the help of templates.
    2. Power BI Services – Power BI Services is a Service-as-a-platform or a cloud based service.
    3. Power BI Mobile App – The Power BI App is available for iOs, Android, and Windows.

   

