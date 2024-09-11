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
 - select dname,sum(sal) from [dbo].[emp],[dbo].[dept] where emp.deptno=dept.deptno group by dname
4. Who is top sal employee?
 - King(5000)


