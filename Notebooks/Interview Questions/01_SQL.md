1. Write Basic Sql **Statements**?

	In Sql Statement we should have **select/from/where/group by/having/order by**
1. Write Sql for Total Sal dept name wise ?

	Select dname,sum(sal) as totalsal
	from emp,dept
	where emp.deptno=dept.deptno
	group by dname
1. Can we get all salesmans information where dept name is Sales?

	select * from emp,dept where emp.deptno=dept.deptno and dept.deptno=30 and job = 'SALESMAN'
	
