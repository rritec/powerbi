
- **Power BI Desktop** Key Components
    1. Power Query Editor
        - Connecting Data Sources
            - Files(Excel ... etc)
            - Relational Databases (MySql,MS Sql Server ... etc)        - 
        - Import Tables
        - Transformations
            - Replace **null** with **zero**
            - Add new column
            - Change datatype
            - Filter data
            - .... etc        
        - Understanding Transformations in M-Language of Power BI
        - Combine
            - Append(Union All)
            - Merge(Join)
                - Inner Join
                - Left Outer Join
                - Right Outer Join
                - Full Outer JOin
                - Left Anti Join
                - Right Anti Join 
        - Based on these concepts let us do one small project
    1. Power Pivot
    1. Power View
    
# Lab Overview

## SCENARIO
ABC is a company that manufactures and sells **sporting goods**. The company has offices in the United States (US) and several other countries. Its sales comprise of US sales and International sales. ABC’s sales come from its owned manufactured products, as well as other manufacturers’ products.

ABC's US office stores the sales data on an **Access** database. ABC International sales transactions are available as **Comma Separated Values (CSV)** files. They could be generated daily, either manually by someone, or automatically by an automated process. They are available in a dedicated folder. These CSV files have the same column structure as the sales table for the US sales that comes from the SQL Database.

You want to perform analysis on ABC's worldwide sales data for the year **2000 to 2015**. You need to bring all these data into Power BI Desktop before you can perform any analysis. Finally, you want to compare ABC's **country sales with the country population**. You need to import the country population data from a less structured **Excel** report to Power BI.



## LAB OVERVIEW

This lab comprises of three exercises:

In the **First Exercise**, you will import data to Power BI Desktop from an Access database file.

In the **Second Exercise**, you will import data from CSV files which resides in a file folder. You will append this new data to the corresponding existing data that comes from the Access Database.

In the **Third Exercise**, you will import data to Power BI Desktop from an Excel file that is less structured.



## WHAT YOU'LL NEED

A computer with the latest version of Power BI Desktop installed on it.

A copy of the `Access Database` containing ABC's US sales data.

`4 CSV files`, containing ABC’s international sales data:

1. CA Sales.csv
2. FR Sales.csv
3. DE Sales.csv
4. MX Sales.csv

An `Excel` file containing country population data.

## Import Data from Access Database


1. Open `Power BI Desktop`.
2. Click `Get Data`.
3. Click `Access database`, and click `Connect`.
4. Navigate to `LabData`, click `PowerBI.accdb`, and click `Open`.
5. Select `bi_date, bi_geo, bi_manufacturer, bi_product` and `bi_salesFact` and click `Transform`.
6. In Queries, select `bi_salesFact`.
7. Select the `Date` column.
8. Click the `Transform` ribbon.
9. In the `Any Column` group, select `Data Type` and select `Date`.
10. Click the drop-down button at the top of the `Date` column.
11. Click `Date` Filters and click `After`.
12. In the first Enter or select a value field, type 12/31/1999 if you are using MM/DD/YYYY dates and 31/12/1999 if you are using DD/MM/YYYY dates and click OK.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0092.png?raw=true)
    
13. In `Queries`, select `bi_Date`.
14. Select the Date column.
15. Click the Transform ribbon.
16. In the Any Column group, select Data Type and select Date.
17. Click the drop-down button at the top of the Date column.
18. Click Date Filters and click After.
19. In the first Enter or select a value field, type 12/31/1999 if you are using DD/MM/YYYY dates and 31/12/1999 if you are using DD/MM/YYYY dates and click OK.
20. Rename the queries as follows:

- In Queries, right click **bi_date**, click Rename, replace the text with **Date**, and press Enter.
- In Queries, right click **bi_geo**, click Rename, replace the text with **Locations**, and press Enter.
- In Queries, right click **bi_manufacturer**, click Rename, replace the text with **Manufacturers**, and press Enter.
- In Queries, right click **bi_product**, click Rename, replace the text with **Products**, and press Enter.
- In Queries, right click **bi_salesFact**, click Rename, replace the text with **Sales**, and press Enter.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0094.png?raw=true)
    
21. Click the Home ribbon.
22. Click **Close and Apply**.
23. Click **Data** and explore the imported data in the Data View.

## Import Data from a Folder Containing CSV Files

Continue with your Power BI file from the previous exercise. You want to create a Query for the International sales and append the Query to the Query from US Sales.

1. On the **Home** ribbon, click **Get Data** > click **File** > Click **Folder** > click **Connect**.
1. In Folder path, go to **labdata/Lab1** and select **International** folder, and click **OK**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0095.png?raw=true)

1. Click on **Combine & Transform Data**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0096.png?raw=true)

1. Observe data > Click on **ok**
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0097.png?raw=true)    

1. In **QUERY SETTINGS** change the name to **International Sales**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0098.png?raw=true) 
    
1. Select the **Date** column.
1. Click the **Transform** ribbon.
1. In the **Any Column** group, select **Data Type** and select **Date**.
1. Click the drop-down button at the top of the **Date** column.
15. Click **Date Filters** > click **After**.
16. In the first Enter or select a value field, type **12/31/1999** if you are using DD/MM/YYYY dates
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0099.png?raw=true)
    
17. In **Queries**, select **Sales**.
18. On the **Home** ribbon, click **Append Queries**.
19. Select **International Sales** and click **OK**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0100.png?raw=true)
    
20. On the **Add Column** ribbon > Click on **Custom Column**.
21. In New column name type **Country Name**.
22. To replace null values with USA, in Custom column formula, type the following formula and click OK:
`=if [Country] = null then "USA" else [Country]`
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0101.png?raw=true)
    
    
23. Right-click the header of the **Country** column and click **Remove**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0102.png?raw=true)
    
24. Click the **Home** ribbon.
25. Click **Close & Apply**.
26. Click **Data** and explore the imported data in the **Data View**.

## Import a Less Structured Data from an Excel File
 

Continue with your Power BI file from the previous exercise. You want to import an Excel report containing population data for the countries that VanArsdel operates.

1. Import the data from the file folder by clicking **Get Data** > **Excel** > **Connect**.
1. Select **..Labdata/lab1/Country Population by Year.xlsx** and click **Open**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0103.png?raw=true)

1. Select **Sheet1** and click **Transform Data**.
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0104.png?raw=true)    
    
1. In **QUERY SETTINGS** change Name to **Country Population**.
1. On the ribbon, click **Remove Rows** > Click **Remove Top Rows** > in **Number of rows** >  type **3** > click **OK**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0105.png?raw=true)
    
1. On the ribbon, click Use **First Row as Headers**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0106.png?raw=true)    
1. Select the **1999** column, hold **Shift** and select the **2014** column.
1. On the **Transform** ribbon, click **Unpivot** Columns.
1. Right-click the **Attribute** column header and click **Rename**.
1. Type **Year** and press **Enter**.
1. Right-click the **Value** column header and click **Rename**.
1. Type **Population** and press **Enter**.
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0107.png?raw=true)
    
1. Click the **drop-down** button on the **Year** header, unselect **1999**, and click **OK**.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0108.png?raw=true)
    
1. Click the **Year** header, on the **Transform** ribbon click **Data Type**, and click **Whole Number**.
1. Click the **Population** header, on the **Transform** ribbon click **Data Type**, and click **Whole Number**.
1. Click the **Home** ribbon.
1. Click **Close & Apply**.
1. Load the **data** into Power BI Desktop.
1. Explore the imported data in the Data View.


## Questions
-----
1. How Many Types of connections available in **Power BI**
    - Import
    - DirectQuery
    - Live Connection
    - Streaming Connection
2. What is difference between Import and Direct Connection?
    1. Import:
        - Gives you the **full suite** of transformation and **data manipulation** in the Desktop
        - There is a 1 GB limit to the Desktop if you plan on publishing to the PBI Service
        - Scheduling Datasets using gateway is needed to avoid old(stale) data
    2. DirectQuery:
        - Limits your ability to manipulate data in the Desktop (removes the Data section)
        - Leaves the data in the SQL database
        - Is "live", no need to schedule a refresh (In the Service)
2. What is the max data limit in a given dataset?

    - **1 GB**
    
    - for more information read this [doc](https://docs.microsoft.com/en-us/power-bi/admin/service-admin-manage-your-data-storage-in-power-bi#:~:text=There%20is%20a%201%20GB,250%20MB%20for%20the%20dataset)
1. How Power BI define datatypes?
    - Based on first 200 rows data values


```python

```
