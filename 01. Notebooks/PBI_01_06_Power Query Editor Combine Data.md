
# Combine Queries
- In power BI, we can combine data into two ways
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
1. Can you show null measures corresponding rows in the report?
   
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
