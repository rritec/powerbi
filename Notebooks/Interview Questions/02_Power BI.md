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

    * Dataset is a collection of data gathered from various sources like SQL Server, Azure, Text, Oracle, XML, JSON, and many more. With the GetData feature in         Power BI, we can easily fetch data from any data source.

47. What is Report ?

    * Reports are a structured representation of datasets that consists of multiple pages. Reports help to extract important information and insights from               datasets to take major business decisions.

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

53. What is row-level security?

    Row-level security limits the data a user can view and has access to, and it relies on filters. 
    Users can define the rules and roles in Power BI Desktop and also publish them to Power BI Service to configure row-level security.
    
54. Define bi-directional cross filtering?

    Bidirectional cross-filtering enables them to apply filters on both sides of a table relationship. 
    You can apply the filters by propagating the filter context to a second related table on the other side of a table relationship.

55. What is "M language"?

    M is a programming language used in Power Query as a functional, case-sensitive language similar to other programming languages and easy to use.

56. What are the major differences between visual-level, page-level, and report-level filters in Power BI?

    Visual-level filters are used to filter data within a single visualization. Page-level filters are used to work on an entire page in a report, and 
    different pages can have various filters. 
    Report-level filters are used to filter all the visualizations and pages in the report.

57. What are KPIs in Power BI?

    KPI is abbreviated as Key Performance Indicator. Any professional organization has teams and employees follow the KPI protocols. The organizations set 
    up KPIs for all the employees. These KPIs act as their targets. These KPIs are compared to previous performance and analyze the progress.

58. What is the incremental refresh in the context of Power BI?

    Incremental refresh is used to refresh the newly added data to avoid truncating and loading data.

59. What are the different joins in Power BI?

    1.Horizontal Joins to append data from multiple tables
    2.Vertical Joins to merge the data from multiple tables

60. Divide Function Vs Divide Operator
- It's recommended that you use the **DIVIDE function** whenever the denominator is an expression that could return zero or BLANK.
- In the case that the denominator is a **constant value**, we recommend that you use the **divide operator**. In this case, the division is guaranteed to succeed, and your expression will perform better because it will avoid unnecessary testing.
- [Refer document](https://learn.microsoft.com/en-us/dax/best-practices/dax-divide-function-operator)
61. Table 1 has one column and 4 rows with values 1,1,0,null and Table2 has one column with values 1,1,null,null then let me know how many rows we will get in full outer join? left outer join? reight outerjoin?inner join? ca you get full outer join results without using full outer join ?
``` sql


Create Table DATATableA
(
ColumA Varchar(20),
integrationid int,
)


Insert into DATATableA(ColumA,integrationid) Values ('1',1)
Insert into DATATableA(ColumA,integrationid) Values ('1',2)
Insert into DATATableA(ColumA,integrationid) Values ('0',3)
Insert into DATATableA(integrationid) Values (4)


Select * From DATATableA;



Create Table DATATableB
(
ColumB Varchar(20),
integrationid int,
)
Insert into DATATableB(ColumB,integrationid) Values ('1',1)
Insert into DATATableB(ColumB,integrationid) Values ('0',2)
Insert into DATATableB(integrationid) Values (3)
Insert into DATATableB(integrationid) Values (4)


Select * From DATATableB;



Select DATATableA.ColumA,DATATableB.ColumB  from DATATableA
Full OUTER JOIN DATATableB ON DATATableA.ColumA = DATATableB.ColumB;


```

![image](https://github.com/rritec/powerbi/assets/20516321/1bb17dbe-1a73-42f2-ac7f-ebcbf733d9bc)

62. split below data in power query to get two columns
- SAR:98
- IND-560
- RAND_:9854
- AED=78
63. Get domain name from mail ids using SQL and PowerBI
64. write query to get duplicate rows 
65. reverse the ddmmyyyy into yyyymmdd in sql and powerbi.

   






	






  
    
