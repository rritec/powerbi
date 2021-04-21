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
        
1. **Power BI Desktop - Power View - Visualization**
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
    •	Overview of Dashboards and Service
    
    •	Uploading to Power BI Service
    
    •	Quick Insights
    
    •	Configuring a Dashboard
    
    •	Adding Textbox, Image Widgets
    
    •	Featured and Favorite Dashboard
    
    •	Filtering Dashboard
    
    •	Dashboard Settings
    
    •	Natural Language Queries
    
    •	Featured Questions
    
    •	Sharing a Dashboard
    
    •	In-Focus Mode
    
    •	Pinning a Live Page
    
    •	Custom URL and Title
    
    •	TV Mode and Collapse Navigation
    
    •	Printing Dashboard and Exporting Data
    
    •	Export to CSV and Excel
    
    •	Power BI Notifications
    
    •	Alerts in the Power BI Service
    
    •	Personal Gateway
    
    •	Publishing to Web
    
    •	Admin Portal
    
    •	Viewing in Windows App
    
    •	Viewing in Android App
    
    •	Viewing in iPad
    
    •	 Upload PBI Report and Pin Visualizations
    
    •	Share Dashboard and Update Report
    
    •	Schedule Data Refresh
    
1. **Working with Excel**

    •	Introduction
    
    •	Importing Excel Data using Simple Table
    
    •	Excel Workbook with Excel Data Model
    
    •	Connecting to Excel Workbook on OneDrive for Business
    
    •	Pinning Excel Tables or Visuals
    
    •	Analyzing Data in Excel
    
1. **Direct Connectivity**

    •	Direct Connectivity to SQL Database
    
    •	Direct Connectivity to SSAS
    
    •	Using SSAS Connector
    
    •	SSAS Multi Dimensional Preview
    
    •	SAP HANA
    
    •	Direct Connectivity From Power BI Desktop
    
    •	Direct Connectivity From Power BI Service
    
1. **Developer API**

    •	Introduction
    
    •	Interactive API Console
    
    •	Registering a Client App and Embedding a Tile
    
    •	Integrating a Tile to Your App
    
    •	Using PubNub to Push Data to a Tile
    
    •	Creating Custom Visuals
    
    •	Using Custom Visuals
    
    •	Power BI Embedded
    
1. **Mobile App**

    •	Introduction
    
    •	Report Gallery and Search
    
    •	Mobile Dashboard Layout
    
    •	Sharing and Annotating in Power BI Mobile
    
    •	Taking Your Mobile Content Offline
    
    •	Platform Specific Features
    
    •	Search and Recent
    
    •	Limiting Access to Mobile + MAM
    


