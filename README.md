# Power BI
This Repository has **Power BI** Training Materials developed by **Myla Ram Reddy**.

Please contact my HR **Renuka** for **Training and Certification** @ **8374899166**(whatsapp)

----

Gain a 360° of how to explore and use Power BI to build impactful reports. In this course, you’ll go from **zero** to **hero**, as you discover how to use this popular business intelligence platform through **hands-on exercises**. You’ll first learn how to confidently load and transform data using Power Query and the importance of data models, before diving into creating visualizations using Power BI’s drag-and-drop functionality. You’ll also learn how to drill-down into reports and make your reports fully interactive. Lastly, you'll level-up your skills using **DAX formulas** (Data Analysis Expressions) to create customized calculated columns and fields to better analyze your data. Get started now. You've got the power!

---
**Course Content**

---


1. Introduction
	- What is Power BI?	
	- What is Power Apps?
	- What are the different BI tools available?
	- Why Power BI?
	- Products of Power BI
	- What is Power BI Desktop?
	- What is Power BI Service?
	- What is Power BI Mobile?
	- What is M-Language?
	- What is DAX?
1. Data Warehousing Concepts
	- What is OLTP
	- What is Data warehouse
	- Difference between OLTP Vs OLAP
	- Difference among Primery Key/Foriegn Key/Surrogate Key
	- Types of Tables
		- Dimension Tables
		- Fact Tables
	- Types of Schemas
		- Star Schema
		- Snow Flake Schema
		- Mixed Schema	
1. Power BI Desktop
	- Introduction to Power BI Desktop
	- Power BI Desktop Components
		- Power Query Editor
		- Power Pivot
		- Power View
1. Power Query Editor
	- Connecting to new Source
		- File connections (Excel,Csv,XML,JSON,Folder)
		- Connecting to Databases (MySql,MSSqlServer,Access dtatabase,...etc)
		- Cloud Connections(SnowFlake Database)
		- Online Connections(Web,Github ..etc)
	- Importing Tables
	- Types of Connections
		- Import
		- Direct
		- Live Connection		- 
	- Basic Transformations
		- Changing datatypes
		- replacing nulls with zero
		- concatnating columns
		- spliting columns
		- renameing columns
		- observing transformation steps
		- understanding M-Language
		- Computed columns/calculations
	- M-Language
		- About Let and In
		- Single Line comments in M-language
		- Multi line comments
		- How to write M-language code in multiple lines
		- Change Steps in Query settings and observe in M-language
		- Change M-language and observe Query Setting Steps
		- Build Query using M-Language Script from Blank Query
	- Combine Queries
		- Append
			- Learn SQL Queries of union ,Union all,Minus 
			- Prove Power BI Append is equal to Union all			
		- Merge
			- Inner Join
			- Left Outer Join
			- Right Outer Join
			- Full Outer Join
			- Left Anti Join
			- Right Anti Join
		- Learn how to implement Cross join,Non equi join.
		- Learn SQL Queries of Joins
	- Query Folding
		- How to see Native Query
	- Project 1: Power Query Editor Level Project
		- Import Data from Access Database
		- Import Data from a Folder Containing CSV Files
		- Import a Less Structured Data from an Excel File
	
1.  **Power BI Desktop - Power Pivot - Modelling**
	- Introduction
	- What is Relationship?
	- What is Cardinality
	- Types of cardinality
	- What cardinality is used between fact and dimension tables and why?
	- Can we use many to many cardinality? if we want to skip what are the workarounds?
	- Can we use one to one cardinality? if we want to skip what are the workarounds?
	- What is active relationship/join?
	- What is inactive Relationship/Join
	- When to go for Inactive relation ships? 
	- What is role playing dimension? Can we use active and inactive both between role playing dimension and fact
	- What is Cross Filter Direction?
	- Types of Cross Filter Directions?
	- What type of direction used in star schema?
	- When to go for Both direction?
1.  **Power BI Desktop - Power Pivot - Data Analysis Expressions(DAX)- Calculations**
	- Introduction	
	- When to go for new column
	- When to go for New Mesure
	- New column Vs New Measure
	- What is Implicity Mesure
	- What is Explicity Mesure
	- What is compound Mesure
	- What is Computed column?
	- Date and time functions
		- CALENDAR
		- CALENDARAUTO
		- DATE
		- DATDIFF
		- DATEVALUE
		- NOW
		- TODAY
		- CALENDAR Vs CALENDARAUTO
		- NOW Vs TODAY
		- ... etc
	- Information functions
		- USERNAME
		- USERPRINCIPALNAME
		- USERNAME Vs USERPRINCIPALNAME
		- ISBLANK
		- ISEMPTY
		- ISBLANK Vs ISEMPTY
		- HASONEVALUE
		- ... etc
	- Logical functions
		- IF
		- IFERROR
		- AND
		- ... etc
	-  Math and trig functions
		- DIVIDE
		- DIVIDE Vs /
		- TRUNC
		- ROUND
		- ... etc
	-  Relationship functions
		- CROSSFILTER
		- USERELATIONSHIP
	-  Statistical functions
		- Explain Itterator Functions
		- sumx
		- countx
		- minx
		- maxx
		- rankx
		- SUM Vs SUMX
		- COUNT Vs COUNTX
		- COUNTA Vs COUNTAX
		- COUNT Vs COUNTA
	- Filter functions
		- ALL
		- FILTER
		- SELECTEDVALUE
		- CALCULATE
		- CALCULATETABLE
		- Difference between Calculate Vs Calculatetable
		- REMOVEFILTERS
		- ...etc
	- Time intelligence functions
		- SAMEPERIODLASTYEAR
		- TOTALYTD
		- ...etc
	- Explain DAX Statements
		- Define
		- Evalute
		- Var
		- Order By	- 
	
1.  **DAX Studio**
	- Introduction
	- Installation
	- What are Power BI External Tools
	- Open Power BI Model in DAX Studio
	- What is DAX Query
	- See Dax Query using Performance Analyser tool
	- SQL Query Vs DAX Query
	- Write Few Queries from Scratch
		- select * from Customer Vs EVALUATE Customer
		- select city from customer Vs EVALUATE VALUES(Customer[City])
		- select * from customer where city ="redmond" Vs EVALUATE CALCULATETABLE ( Customer, Customer[City] = "Redmond" )
		- ... etc
	- Project 2: Power Pivot Level Project
		- Manage Table Relationships
		- Last Year Comparison
		- Year to Date
		- Market Share
		- Optimize the Data Model
        
1. **Power BI Desktop - Power View - Report - Visualization**
	- Introduction
	- Hierarchy
		- Creating hierarchy
		- Drill down
		- Drill Up
		- Show Next Level
		- Expand Next Level
		- Drill Through
		- Back button
		- customise back button and use userdefined image as back button
	- Filters
		- Viz level filter
		- page Level Filter
		- All pages or Report level Filter
		- Drill through Filter
		- Slicer
		- Row Level Security(RLS)	- 	- 
	- Visulizations
		- Slicer
		- Table
		- Matrix
		- Column Chart
		- Bar Chart
		- Pie
		- Donut
		- Treemap
		- Bar Chart with Line
		- Waterfall 
		- Scatter Chart
	- Project 3: Power View Level Project
		- Page Layout and Formatting
		- Visual Relationship
		- Duplicate Page
		- Categories with No Data
		- Default Summarization and Categorization
		- Positioning, Aligning, and Sorting Visuals
		- Custom Hierarchies
		- Python - Visual Integration
		- Cross-Tabular Report
		- Part-to-Whole Report
		- Relationship Report
		- Trend Report
		- Rank Report
    
1. **Power BI Service**
	- Introduction
	- Signup and access [app.powerbi.com](app.powerbi.com)
	- Workspace
		- Create Workspace
		- Publish PBIX to workspace
		- Upload PBIX to workspace
	- Dashboard
		- Create Dashboard
		- Pin Viz to Dashboard
		- Pin Entire page to dashboard
		- Pin Vs Pin Live
		- Share Dashboard
		- Edit Dashboard
		- Tiles
			- Web Content Tile
			- Image Tile
			- Text Tile
			- Video Tile
		- Dashboard Layouts
		- Dashboard Mobile View
		- Dashboard Web View
		- Featured and Favorite Dashboard
		- Filtering Dashboard
		- Dashboard Settings
		- Q&A - Natural Language Queries - NLP
		- Printing Dashboard and Exporting Data
		- Export to CSV and Excel
	- Apps
		- Creating App
		- Updating App
		- Controling reports visibility in app
1. **Power BI Gateways**
	- Introduction
	- What is Gateway
	- Types of Gateways
	- Personal Gateway
	- Standalone or enterprise gateway
	- Installation of Gateway
	- Configuring Gateway
	- Scheduling
		- Refreshing Dataset daily 8 times in Pro licence
		- Refreshing Dataset daily 48 times in Premium licence
		- Refreshing dateset weekly
		- Updateing source credentials of dataset
	- Incremental Refresh
		- RangeStart
		- RangeEnd
		- Refresh only last 10 days data
1. **Power BI Connections**
	- Import
	- Direct
	- Live
	- Streaming
	- Difference among above **4** connections
1. **Power BI Performance Tunning**
	- Performance Analyser
	- Query Folding
	- Index
	- Dax Formulas tuning
1. **Power BI Security**
	- Authentication
	- Object Level Authrization
		- Admin
		- Member
		- Contributor
		- Viewer
	- Row Level Security
		- Static
		- Dynamic	- 
1. **Power BI Cmdlets and Rest APIs**
	- Install Cmdlets
	- Connect power BI
	- Disconnect Power BI
	- Get list of workspaces
	- Get list of users
	- Add user to workspace
	- Remove user from workspace
	- Create New Workspace
	- Export list of reports
	- Export list of dashboards

    

    


