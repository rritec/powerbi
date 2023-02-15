# Power BI
1. **[Introduction](#Introduction)**<br>
2. **[Power BI Desktop](#Power-BI-Desktop)**<br>
3. **[Working with MySql](#Working-with-MySql)**<br>
4. **[Working with SQL Server](#Working-with-SQL-Server)**<br>
5. **[M-Language](#M-Language)**<br>
6. **[Combine Queries](#Combine-Queries)**<br>
7. **[Power Query Editor Project](#Power-Query-Editor-Project)**<br>
8. **[Power Pivot Modeling part 1](#Power-Pivot-Modeling-part1)**<br>
9. **[Power BI Desktop](#Power-BI-Desktop)**<br>
10. **[Power BI Desktop](#Power-BI-Desktop)**<br>
11. **[Power BI Desktop](#Power-BI-Desktop)**<br>
12. **[Power BI Desktop](#Power-BI-Desktop)**<br>
13. **[Power BI Desktop](#Power-BI-Desktop)**<br>
14. **[Power BI Desktop](#Power-BI-Desktop)**<br>
15. **[Power BI Desktop](#Power-BI-Desktop)**<br>
16. **[Power BI Desktop](#Power-BI-Desktop)**<br>
17. **[Power BI Desktop](#Power-BI-Desktop)**<br>
18. **[Power BI Desktop](#Power-BI-Desktop)**<br>
19. **[Power BI Desktop](#Power-BI-Desktop)**<br>
20. **[Power BI Desktop](#Power-BI-Desktop)**<br>
21. **[Power BI Desktop](#Power-BI-Desktop)**<br>
22. **[Power BI Desktop](#Power-BI-Desktop)**<br>
23. **[Power BI Desktop](#Power-BI-Desktop)**<br>
24. **[Power BI Desktop](#Power-BI-Desktop)**<br>
25. **[Power BI Desktop](#Power-BI-Desktop)**<br>
26. **[Power BI Desktop](#Power-BI-Desktop)**<br>
27. **[Power BI Desktop](#Power-BI-Desktop)**<br>
28. **[Power BI Desktop](#Power-BI-Desktop)**<br>
29. **[Power BI Desktop](#Power-BI-Desktop)**<br>
30. **[Power BI Desktop](#Power-BI-Desktop)**<br>


# Introduction
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
    
# Power BI Desktop
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


# Working with MySql

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
# Working with SQL Server
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
 



# Combine Queries
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




# Power Query Editor Project

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




# Power Pivot Modeling part 1

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
