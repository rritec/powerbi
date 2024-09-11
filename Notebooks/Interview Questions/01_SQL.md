1. Write Basic Sql **Statements**?

	In Sql Statement we should have **select/from/where/group by/having/order by**
1. Write Sql for Total Sal dept name wise ?

	``` sql
        Select dname,sum(sal) as totalsal
	from emp,dept
	where emp.deptno=dept.deptno
	group by dname
 ```
![image](https://github.com/user-attachments/assets/2951ce02-bc86-4efc-9eff-f5432c1fe1b0)

1. Can we get all salesmans information where dept name is Sales?

	``` sql
select 
	* 
from 
	emp,dept 
where 
	emp.deptno=dept.deptno and 
	dept.dname='SALES' and 
	job = 'SALESMAN'
```
![image](https://github.com/user-attachments/assets/e5f23b0b-641c-442c-bb75-67e8987b7b8d)

1. Write query to get studentname,teachername,subjectname based on below data.

```sql
Create table dbo.student(
Student_ID int,
Student_Name Varchar(50),
Class int)

Create table dbo.TEACHER(
TID int,
Teacher_Name Varchar(50),
)

create table dbo.SUBJECT(
Sub_Id int,
Sub_Name Varchar(50))

create table dbo.STUDENT_SUBJECT(
Stu_Id int,
Sub_Id int,
Teacher_Id int)

Create table dbo.Student_Marks(
Student_ID int,
Sub_Id int,
Marks int,
Class int)

INSERT INTO dbo.student (Student_ID, Student_Name,Class) VALUES
(1, 'aaa',1),
(2, 'bbb',2);

INSERT INTO dbo.TEACHER (TID, Teacher_Name) VALUES
(1, 'hhh'),
(2, 'gggg');

INSERT INTO dbo.SUBJECT (Sub_Id, Sub_Name) VALUES
(1, '2maths'),
(2, 'Science');

INSERT INTO STUDENT_SUBJECT (Stu_Id, Sub_id, Teacher_Id) VALUES
(1, 1, 1),
(2, 1, 1);

INSERT INTO Student_Marks (Student_ID, Sub_Id, Marks, Class) VALUES
(1, 1, 34, 1),
(1, 2, 90, 1),
(2, 1, 55, 1),
(2, 2, 40, 1);
```
``` sql
SELECT
    st.Student_Name,
    T.Teacher_Name,
    Sb.Sub_Name,
    sm.Marks,
    CASE
        WHEN sm.Marks >= 0 AND sm.Marks < 35 THEN 'Fail'
        WHEN sm.Marks >= 35 AND sm.Marks < 50 THEN 'Just Pass'
        WHEN sm.Marks >= 50 AND sm.Marks < 60 THEN 'Second Class'
        WHEN sm.Marks >= 60 AND sm.Marks <= 100 THEN 'First Class'
    END AS Grade
FROM
    STUDENT_SUBJECT ss
JOIN
    STUDENT st ON st.Student_ID = ss.Stu_Id
JOIN
    TEACHER T ON T.TID = ss.Teacher_Id
JOIN
    SUBJECT sb ON sb.Sub_Id = ss.Sub_id
JOIN
    Student_Marks sm ON sm.Sub_Id = ss.Sub_id AND sm.Student_ID = st.Student_ID;
```



2. Find grand total,running total and deptno wise running total
 ``` sql

select deptno,empno,sal,
sum(sal) over () as grand_total,
sum(sal) over (order by deptno,sal) as running_total,
sum(sal) over (partition by deptno order by deptno,sal) as dept_running_total
from emp order by deptno,sal

   ```
4. How we can merge two tables in sql by using merge
5. How to execute Stored procedure in adf
6. How to get alerts in adf ( if we have 100 pipelines if any one pipeline fails we should get alert)
7. In Storage Account have 100 files we should load files by having some specific conditions into Azure Blob storage
8. How to Execute table writtening function
9. How to return value from Stored Procedure
10. How to write data into sql server using pyspark
11. how to remove duplicates from dataframe
12. how to join two dataframes in pyspark
13. If stored procudure value is True then run copy activity else do not run.
14. How to call value writtening function in select query.
15. 
	
