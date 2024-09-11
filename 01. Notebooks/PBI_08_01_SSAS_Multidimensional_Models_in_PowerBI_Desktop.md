
# SSAS Multidimensional Models(Cubes)

## MSBI

    - SSIS > ETL
    - SSRS > Reporting
    - SSAS > Tabular Cube or Multidimensional Cube

## Download and Restore Sample Data

1. Download Sample Data warehouse data **AdventureWorksDW2012.bak**

    https://github.com/Microsoft/sql-server-samples/releases/download/adventureworks/AdventureWorksDW2012.bak

1. Restore Data by following below steps

    https://docs.microsoft.com/en-us/sql/samples/adventureworks-install-configure?view=sql-server-ver15#restore-backup

## Install SQL Server Analysis Services
1. Start > Microsoft SQL Server 2019 > SQL Server 2019 Installation Center (64-bit)
1. Click on Installation > New Sql Server Stand alone installation or add Features to existing installation> select c drive > sql2019 folder > Developer_enu
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0139.png?raw=true)
1.  Select Add fetures to an existing instance
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0140.png?raw=true)
1. Select Analysis Service
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0141.png?raw=true)
1. Follow the wizard    



## Learn Basic of SSAS
1. Setup prerequisites

    https://docs.microsoft.com/en-us/analysis-services/multidimensional-tutorial/multidimensional-modeling-adventure-works-tutorial?view=asallproducts-allversions#prerequisites

1. Complete at least first 2 chapters 

    https://docs.microsoft.com/en-us/analysis-services/multidimensional-tutorial/multidimensional-modeling-adventure-works-tutorial?view=asallproducts-allversions

## Deploy Cube
1. Open **SQL Server Data Tools for Visual Studio 2012** > **File** > **Open** > **Project/Solution** > **Lesson 10 Complete** > select **Analysis Services Tutorial.sln** > Click on **open**
1. In **Solution Explorer** > Right click on **Analysis Services Tutorial** > Click on **Deploy**

## Develop PBI Report using Cube
1. Open **PBI Desktop** > **Get Data**> **SQL Server Analysis Service Database**
1. Provide **Server** as **localhost** > Select **Connect Live** > Click on **ok**
1. Expand **Analysis Service Tutorial** > Select **Sales Summary** > Click on **ok**
1. Select **Calendar Date** Hierarchy and **Total Sales Amount**
1. Observe Report
1. Similarly Develop some other reports


## Optional
- Lear SSIS by using MSFT documents
    - https://docs.microsoft.com/en-us/sql/integration-services/lesson-1-create-a-project-and-basic-package-with-ssis?view=sql-server-ver15-  
- SSRS
    - https://docs.microsoft.com/en-us/sql/reporting-services/install-windows/install-reporting-services?view=sql-server-ver15
    - https://docs.microsoft.com/en-us/sql/reporting-services/reporting-services-tutorials-ssrs?view=sql-server-ver15



```python

```
