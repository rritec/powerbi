1. Write Basic Sql **Statements**?

	In Sql Statement we should have **select/from/where/group by/having/order by**
1. Write Sql for Total Sal dept name wise ?

	Select dname,sum(sal) as totalsal
	from emp,dept
	where emp.deptno=dept.deptno
	group by dname
1. Can we get all salesmans information where dept name is Sales?

	select * from emp,dept where emp.deptno=dept.deptno and dept.deptno=30 and job = 'SALESMAN'
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



2. 
	
