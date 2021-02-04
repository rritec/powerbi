
# Combine Queries
---
- Append
    - Rows appending
    - Append rules
        - Rule 1: The number of columns in each table is same
        - Rule 2: The positions of columns must be same
        - Rule 3: The respective columns data types shoud be same 

- Merge
    - Joins

## Append

- **Scenario:** Append emp10,emp20 and emp30 tables as **emp102030**

### Sql Query


SELECT * INTO [dbo].[emp10] FROM [dbo].[EMP] WHERE DEPTNO=10;

SELECT * INTO [dbo].[emp20] FROM [dbo].[EMP] WHERE DEPTNO=20;

SELECT * INTO [dbo].[emp30] FROM [dbo].[EMP] WHERE DEPTNO=30;


select * from emp10 -- 3 rosws

union

select * from emp20 -- 5 rosws

union

select * from emp30 -- 6 rosws

### Develop Report using Append homogeneous Sources

1. Open **Power BI** > Click on **Get Data** > Select **Databases**> Select **SqlServer** > Click on **Connect** > Provide **Servername** as **localhost** and **Database Name** as **rritec** > Click on **ok**
1. In **Navigator** window Select tables **emp10**,**emp20** and **emp30** > Click on **Transform Data**
1. Click on **Append Queries** > **Append Queries as New** > Select radio button **Three or More Tables** > Select required tables and push to right side then click on **ok**



### Develop Report using Append Hetrogeneous Sources

1. In above report import emp30 data from excel **LabData/Lab1/emp30_data_from_excel.XLSX**
1. Combine This Excel emp 30 with SQL Server emp10 and emp20 data



## Merge
1. Inner Join
1. Left outer Join
1. Right Outer Join
1. Full Outer Join
1. Right Anti Join
1. Left Anti Join
1. Non Equi Join
1. Cross Join


### Inner Join

#### Learn Sql Query

Select dname,ename,job,sal \
from emp,dept\
where emp.deptno=dept.deptno

#### Develop PBI Report using inner Join

1. In above Report import **emp** and **dept**
1. Click on **Merge Queries** > **Merge Queries as New** > Select Join Columns as shown below >Select Type of Join as **Inner Join** > click on **ok**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0033.png?raw=true)
1. In **Query Settings** rename **merge1** as **01_Inner_join**
1. Expand Dept Table in the **work Area** and **Select all columns** > Click on **ok** > Understand Result of SQL Query in database and powerI result, Both Must be same

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0034.png?raw=true)

### Left Outer Join

#### Learn Sql Query

Select emp.deptno,dname,ename,job,sal \
from emp left outer join dept \
on emp.deptno=dept.deptno

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

Select dept.deptno,dname,ename,job,sal \
from emp right outer join dept \
on emp.deptno=dept.deptno

#### Develop PBI Report using Right Outer Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **03_Right_outer_Join**
1. Click on  **Source** Settings and change **inner join** as **Right Outer Join** 
1. Click on **ok** 
1. Observe Result

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0036.png?raw=true)

### Full Outer Join

#### Learn Sql Query

Select dept.deptno,dname,ename,job,sal \
from emp left outer join dept \
on emp.deptno=dept.deptno \
union  \
Select dept.deptno,dname,ename,job,sal \
from emp right outer join dept \
on emp.deptno=dept.deptno 

or 

select dept.deptno,emp.deptno,dname,loc,empno,ename,sal \
from [dbo].[EMP] full outer join [dbo].[DEPT] \
on dept.deptno=emp.deptno \

#### Develop PBI Report using Full Outer Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **04_Full_outer_Join**
1. Click on  **Source** Settings and change **inner join** as **Full Outer Join** 
1. Click on **ok** 
1. Observe Result

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0037.png?raw=true)

### Left Anti Join

#### Learn Sql Query

select * from emp \
where deptno not in (select deptno from dept );

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

select * \
from dept \
where deptno not in (select deptno from emp );

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
select ename,sal,grade 
from emp,salgrade 
where sal between losal and hisal

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
select ename,dname,job,sal \
from emp,dept

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0046.png?raw=true)

#### Develop PBI Report using Cross Join

1. In above report, In Queries Pane ,select **01_Inner_join** > Right Click and click on **Duplicate**
1. In Query Settings rename as **05_Left_Anti_Join**
1. Click on  **Source** Settings and change **inner join** as **Left Anti Join** 
1. Click on **ok** 
1. Observe Result

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0047.png?raw=true)

## Home Work: Develop Below reports

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0022.png?raw=true)

## Questions
1. What is composite Key ?

	A composite key is a combination of two or more columns in a table that can be used to uniquely identify each row in the table
	![image](https://www.google.com/imgres?imgurl=https%3A%2F%2Fwww.got-it.ai%2Fsolutions%2Fsqlquerychat%2Fwp-content%2Fuploads%2F2019%2F11%2F0.png.png&imgrefurl=https%3A%2F%2Fwww.got-it.ai%2Fsolutions%2Fsqlquerychat%2Fsql-help%2Fdata-definition%2Fcreate-composite-primary-keys-in-sql-server%2F&tbnid=TuBpwIiJbUTD7M&vet=12ahUKEwjnk-S-85TsAhULgEsFHcdQCkMQMygGegUIARDTAQ..i&docid=Q1-r5NG5hSa9JM&w=758&h=302&q=composite%20key&ved=2ahUKEwjnk-S-85TsAhULgEsFHcdQCkMQMygGegUIARDTAQ)
	
1. Can we merge/Join in power bi with two or more columns?

	Yes. Press Ctrl key and select multiple columns.
	
	*Note:* In *Model* we can not create join based on multiple columns 
	
```python

```
