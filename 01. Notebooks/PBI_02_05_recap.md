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

				
	
		

		
		
