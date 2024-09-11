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
1. Can we reorder Transformation steps in **Query Settings**?
    - Yes
1. What is the extension of Power BI File?
    - .PBIX
1. The calculation in Power Query Editor is called as ?
    - Co**M**uting Column
1. Can you name some of the Power BI supporting Data Types?
    - Whole Number
    - Decimal
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
1. What all are the softwares installed?
    - Power BI Desktop > Report Devlopment
    - MSFT SQL Server > Database
    - MSFT SSMS > Write SQL Queries
    - Adventureworksdw2012 > Sample Data to understand capabilities of MSFT products
2. 
    - answer
