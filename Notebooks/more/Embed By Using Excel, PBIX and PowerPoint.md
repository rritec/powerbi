Open PowerBI Desktop
Import Data From Excel Data Source By Using Our Material 
## Import scott data from excel

![image](https://user-images.githubusercontent.com/20516321/196328872-9932cfa7-18cb-4b14-b609-e87f4d12bda2.png)


1. Go to windows search > type **Power BI** > Open **Power BI Desktop** > Click on **Get Data** > Click on **File** > Click on **Excel**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0081.png?raw=true)
    
1. Click on **Connect** > Select **Labdata/Lab1/scottdata.xlsx** > Click on **open**
1. In **Navigator** select all three tables > Click on **Transform Data**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0082.png?raw=true)

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

## Save the report
1. Go to **File** menu > click on **save** > Select **powerbi_work** folder > name it as **PBI_01_02_Power Query Editor Shape data using Excel as source** > click on **ok**


## Publish the report

1. Open https://app.powerbi.com/
1. Signin with username and password given to you by your instructor
2. In the left Navigation Pane > Click on Workspaces > Click on Create a Workspace > provide workspace name as rritec - workspace > click on Save
3. In **Power BI Desktop** > click on **signin** and pass username and password
4. Click on **publish** > Select above workspace **rritec - workspace** > click on ok
5. Go to **power BI service** > observe report

Open PowerPoint 
Click On Insert
  ![image](https://user-images.githubusercontent.com/20516321/220101062-a1907f77-798c-48f9-a4fb-5f46bec98557.png)
Click On Add-Ins
From Microsoft Store Search On Download Microsoft PowerBI  (Note:- Need to be sign with same accounts in all apps)
  ![image](https://user-images.githubusercontent.com/20516321/220101325-cd966f5a-9dd7-4c0e-88d9-0d82cc5e1b74.png)

Click On Microsoft PowerBI
Goto app.powerbi.com
Open the dataset what we have published earlier
copy the url above what we published the report and paste 
  ![image](https://user-images.githubusercontent.com/20516321/220101774-37a8fd01-59c9-4f48-9806-78430ecf0f37.png)

click on insert
Modify as per our requirements
Click On Save


Now Open Scott Data file in excel
  ![image](https://user-images.githubusercontent.com/20516321/220102841-59c0aff6-7930-47dd-a585-d8a8bbdb952d.png)
Add One Row with Any details and save it
now open PowerBI report and refresh the data
we will get the output what we have updated in the excel file.


