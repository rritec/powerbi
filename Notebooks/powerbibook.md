# Power BI
1. **[Introduction](#Introduction)**<br>
2. **[Power BI Desktop](#Power-BI-Desktop)**<br>
3. 



# Introduction
---

##  What is BI ?
---
1. BI(Business Intelligence) is a processes that convert **Raw Data** into **Meaningful Information**
1. The **meaningful information** drives **profitable business actions**

## Do you know any BI tools?
---
1. Power BI
1. Tableau
1. Cognos
1. Bo
1. OBIEE
1. Domo
1. Qlick View/Sense
... etc

### Out of these all BI tools, which is best? why ?
---
- According to world's leading research and advisory company **Power BI** is best. 
    - [Gartner Report](https://powerbi.microsoft.com/en-us/blog/microsoft-named-a-leader-in-gartners-2020-magic-quadrant-for-analytics-and-bi-platforms/)
    - [Forrester Report](https://info.microsoft.com/ww-landing-Forrester-Wave-Enterprise-BI-platforms-website.html?LCID=EN-US)


    

## What is Power BI?
---
1. Power BI is a business analytics solution that lets you visualize your data and share **insights** across your organization, or embed them in your app or website.
1. Connect to **hundreds of data sources** and bring your data to **life** with **live dashboards** and **reports**.
1. [Visit for more information](https://powerbi.microsoft.com/en-us/what-is-power-bi/)

## Why Power BI?
---
1. Create data dashboards and visualizations in **minutes**
1. Put BI in everyone’s hands—**economically**. Please see the price of Tableau and Power BI    
    - [Power BI Price](https://powerbi.microsoft.com/en-us/pricing/)
    - [Tableau Price](https://www.tableau.com/pricing/teams-orgs#online)
1. Unify **self-service** and enterprise analytics
1. Accelerate big data prep with **Azure**
1. Find answers fast with industry-leading **AI**
1. Get unparalleled **Excel** integration
1. Turn **insights** into **action**
1. **Stream analytics** in **real time**
1. [Visit for more information](https://powerbi.microsoft.com/en-us/why-power-bi/)

## Do you know Power BI products?
---
1. **Power BI Desktop**(Windows based software)
    - Create rich,interactive reports with visual analytics at your fingertips
    - Go from `data` →  `insight` →  `action` with Power BI Desktop
    - Connect to your data, wherever it is
    - Prep and model your data with ease
    - Provide advanced analytics with the familiarity of Excel
    - Create interactive reports customized for your business
    - Power BI Desktop is nothing but three tools of excel 
        - Power Query or Power Query Editor
        - Power Pivot
        - Power View
            - [Read More](https://support.office.com/en-us/article/power-query-overview-and-learning-ed614c81-4b00-4291-bd3a-55d80767f81d)
            
2. **Power BI Service**(MSFT Cloud)
    - Dashboards are developed here
    - Conduct data-driven collaboration
    - Discover insights quickly
    - Get more done with familiar tools
    - Govern your data securely
3. Power BI Mobile
4. Power BI Embedded
5. Power BI Report Server
        

# Install Power BI Desktop
---
- Download software [here](https://www.microsoft.com/en-us/download/details.aspx?id=58494)
- Run the MSI installer and follow the setup steps    

![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation9.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation8.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation7.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation6.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation5.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation4.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation3.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation2.png?raw=true)
![](https://github.com/rritec/powerbi/blob/master/images/powerbiinstallation1.png?raw=true)
[Reference](https://docs.microsoft.com/en-us/power-bi/desktop-get-the-desktop)

# MSFT SQL Server Installation
---

## Install MSFT SQL Server Database
---

1. Download Sqlserver Developer edition [here](https://www.microsoft.com/en-au/sql-server/sql-server-downloads)

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0132.png?raw=true)
    
1. Run below **.exe** file

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0126.png?raw=true)
1. Click on **Basic**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0127.png?raw=true)
1. Click on **Accept**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0128.png?raw=true)
1. Click on **Install**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0130.png?raw=true)
1. Observe connections info

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0129.png?raw=true)  
   

    

## Instal SQL Server Management Studio (SSMS) 
---

1. Download SQL Server Management Studio [here](https://www.microsoft.com/en-au/sql-server/sql-server-downloads)
1. Double Click on exe file

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0133.png?raw=true)
1.   Click on **Install**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0134.png?raw=true)
1.   Click on **Restart**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0136.png?raw=true)   


## Restore sample data
---

1. Follow below link download and restore sample data **AdventureWorksDW2012.bak**
https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15

## Instal MSBI (Download SQL Server Data Tools (SSDT))
---

1. Download Sqlserver Developer edition https://www.microsoft.com/en-au/sql-server/sql-server-downloads

direct link : https://docs.microsoft.com/en-us/sql/ssdt/download-sql-server-data-tools-ssdt?view=sql-server-ver15#ssdt-for-vs-2017-standalone-installer

1. Double Click on exe file

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0136.png?raw=true)
1.   Click on **install**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0137.png?raw=true)
1.   Click on **install**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0138.png?raw=true)   


# MySql Installation(Optional)
---
1. Download the software 
    https://dev.mysql.com/downloads/file/?id=508936
3. Ckick in msi file and install it
![image](https://user-images.githubusercontent.com/20516321/148321034-5bbd5b60-57e6-42c4-ae60-3fb446f6c1b1.png)

4. Click on Next
![image](https://user-images.githubusercontent.com/20516321/148321192-cef7b0f0-d38a-417e-b0a4-3827711da9e3.png)

5. Observe all components
![image](https://user-images.githubusercontent.com/20516321/148321246-8f013719-ee9a-428a-844b-7134cc97aaf0.png)
6. Click on Next
    ![image](https://user-images.githubusercontent.com/20516321/148321730-ebf433d9-08cb-4b66-985e-98d27a9be83b.png)

7. Provide **root** user password and notedown some where
    ![image](https://user-images.githubusercontent.com/20516321/148321849-dff93321-3f00-466c-b3ca-af97b5758a5f.png)




## Interview Questions
-----
1. What are the **key components** of power BI.
    1. Power BI Desktop(Power Query/Power Pivot/Power View)
    2. Power BI Service
    3. Power BI Mobile
    4. Power BI Maps
    5. Power BI Embeded Analytics
    
# Power BI Desktop
    - It has mainly three Components
        - Power Query Editor(Extract + Transforming + Loading into PBIX file)
        - Power Pivot (Model + DAX)
        - Power View or Report View
# Power Query Editor
- It is also known as `Power Query`
# Download all materials and data
1. Download materials [here](https://github.com/rritec/powerbi/archive/refs/heads/master.zip)
1. Create one folder on desktop with the name of **PowerBI_work**
1. Move above **powerbi-master.zip** file to **PowerBI_work** folder
1. Right click on **powerbi-master.zip** file > Click on **Extract All**
1. Observe all materials and Labs


## Import scott data from excel

![image](https://user-images.githubusercontent.com/20516321/196328872-9932cfa7-18cb-4b14-b609-e87f4d12bda2.png)


1. Go to windows search > type **Power BI** > Open **Power BI Desktop** > Click on **Get Data** > Click on **File** > Click on **Excel**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0081.png?raw=true)
    
1. Click on **Connect** > Select **Labdata/Lab1/scottdata.xlsx** > Click on **open**
1. In **Navigator** select all three tables > Click on **Transform Data**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0082.png?raw=true)

## Power Query has `5` main parts
1. Menu Bar(Home/Transform/Add Column/View/Tools/Help)
1. Queries Pane
1. Query Settings Pane
1. Work area
1. Formula Bar

## Replace in `emp` table `comm` column `null` with `0`
1. In **Queries** pane  > Select **emp** table > select **comm** column
1. In the **toolbar** > Click on **Replace Values** > type as shown in below image
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0083.png?raw=true)



## Rename column name `ename` as `Employee Name`
1. In **Queries** pane > select **emp** > Right click on **ename** column 

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0087.png?raw=true)
    
1. Click on **rename** and name it as **Employee Name** > press enter

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0088.png?raw=true)
    
## Create `totalsal` column
1. In the **Menu bar** > Click on **Add Column** > Click on **Custom Column** > Name it as **totalsal**
1. Develop formula as shown in below image > Click on **ok**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0084.png?raw=true)
1. Observe output
   
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0086.png?raw=true)




## Observe Data Types
1. Decimal Number
2. Fixed Decimal Number
3. Whole Number
4. Percentage
5. Date/Time
6. Date
7. Time
8. Date/Time/Timezone
9. Duration
10. Text
11. True/False
12. Binary
## Change data type of TotalSal to decimal numbar
1. Right click on **totalsal** column > click on **Change type** > Click on **Decimal Number**

## AutoFilter/Basic Filter
### Filter `sal` column to display only greater than `900`
1. Click on **sal** column down arrow mark > Click on **Number Filters** > Click on **Greater Than** > type **900** > Click on **ok**

## Save the report
1. Go to **File** menu > click on **save** > Select **powerbi_work** folder > name it as **PBI_01_02_Power Query Editor Shape data using Excel as source** > click on **ok**


## Publish the report

1. Open https://app.powerbi.com/
1. Signin with username and password given to you by your instructor
2. In the left Navigation Pane > Click on Workspaces > Click on Create a Workspace > provide workspace name as rritec - workspace > click on Save
3. In **Power BI Desktop** > click on **signin** and pass username and password
4. Click on **publish** > Select above workspace **rritec - workspace** > click on ok
5. Go to **power BI service** > observe report
    

## Reference 

https://docs.microsoft.com/en-us/power-bi/fundamentals/desktop-getting-started

https://docs.microsoft.com/en-us/power-bi/connect-data/desktop-shape-and-combine-data

https://docs.microsoft.com/en-us/power-bi/transform-model/desktop-common-query-tasks

https://docs.microsoft.com/en-us/power-bi/desktop-add-custom-column

https://docs.microsoft.com/en-us/powerquery-m/power-query-m-function-reference


```python

```
## Questions
1. **Power BI** Key Components?
    - Power BI Desktop
    - Power BI Service
    - Power BI Mobile
1. **Power BI Desktop** Key components
    - Power Query Editor
    - Power Pivot
    - Power View
1. Power Query Editor useing which language?
    - M - Language
1. Can we import 2 sheets from excel workbook which has 5 sheets?
    - Yes
1. Each Sheet is called as what in power Query Editor?
    - Query
1. Can we reorder Transformation steps in **Qurry Settings**?
    - Yes
1. What is the extension of Power BI File?
    - .PBIX
1. The calculation in Power Query Editor is called as ?
    - Co**M**uting Column
1. Can you name some of the Power BI supporting Data Types?
    - Whole Number
    - Deciambal
    - Text
    - Date
    - True/False(Bool)
    - DateTime
    - .... etc
    
1. In how many ways we can see the list of query applied steps?
   - Query setting pane
   - Advance Editor
1. In Excel how many kinds of data containers available?
    - Sheet
    - Table
1. How Many Data Sources/Data bases worked ?
    - Flat Files(Excel,Csv,Tab delimited,Json,XML...etc)
    - Relational Databases (MS Sql Server,Oracle,Teradata,MySql,BigData Hive,...etc)
    - Cloud Databases(Snow Flake,Azure SQl Database,Azure Synapse,Azure Blobs...etc)
