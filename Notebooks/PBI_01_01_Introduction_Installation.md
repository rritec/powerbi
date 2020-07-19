
# Power BI Demo
---

##  What is BI ?
---
1. BI(Business Intelligence) is a processes that convert raw data into meaningful information
1. The meaningful information drives profitable business actions

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


    

## What is Power BI
---
1. Power BI is a business analytics solution that lets you visualize your data and share insights across your organization, or embed them in your app or website.
1. Connect to hundreds of data sources and bring your data to **life** with **live dashboards** and **reports**.
1. [Visit for more information](https://powerbi.microsoft.com/en-us/what-is-power-bi/)

## Why Power BI
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
1. **Power BI Desktop**
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

# MS SQL Installation
---

## Install SQL Server Database
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
1. Test Connection and version

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0131.png?raw=true)     

    

## Instal SQL Server Management Studio (SSMS) 
---

1. Download Sqlserver Developer edition [here](https://www.microsoft.com/en-au/sql-server/sql-server-downloads)
1. Double Click on exe file

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0133.png?raw=true)
1.   Click on **Install**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0134.png?raw=true)
1.   Click on **Restart**

   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0136.png?raw=true)   


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


## optional
---

1. Follow below link download and restore sample data **AdventureWorksDW2012.bak**
https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15

# MySql Installation
---
https://dev.mysql.com/doc/refman/8.0/en/windows-installation.html