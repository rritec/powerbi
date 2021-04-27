
# Power Query Editor
- It is also known as `Power Query`
# Download all materials and data
- https://github.com/rritec/powerbi/archive/refs/heads/master.zip


## Import scott data from excel
1. Open **Power BI Desktop** > Click on **Get Data** > Click on **File** > Click on **Excel**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0081.png?raw=true)
    
1. Click on **Connect** > Select **Labdata/Lab1/scottdata.xlsx** > Click on **open**
1. In **Navigator** select all three tables > Click on **Transform Data**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0082.png?raw=true)

## Power Query has `5` main parts
1. Menu Bar
1. Queries Pane
1. Query Settings Pane
1. Work area
1. Formula Bar

## Replace in `emp` table `comm` column `null` with `0`
1. In **Queries** pane  > Select **emp** table > select **comm** column
1. In the **toolbar** > Click on **Replace Values** > type as shown in below image
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0083.png?raw=true)



## Create `totalsal` column
1. In the **Menu bar** > Click on **Add Column** > Click on **Custom Column** > Name it as **totalsal**
1. Develop formula as shown in below image > Click on **ok**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0084.png?raw=true)
1. Observe output

   
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0086.png?raw=true)

## Rename column name `ename` as `Employee Name`
1. In **Queries** pane > select **emp** > Right click on **ename** column 

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0087.png?raw=true)
    
1. Click on **rename** and name it as **Employee Name** > press enter

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0088.png?raw=true)


## Data Types
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

## AutoFilter/Basic Filter

### Filter `Job` column to display only `MANAGER` and `ANALYST`

### Filter `Hiredate` column to display only greater than `01-Jan-1982`

### Filter `sal` column to display only greater than `2400`

### Filter `Job` and `sal` column to get `managers` info whoms cost to company(CTC) is more than `2500`

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
1.In how many ways we can see the list of query applied steps?
   - Query setting pane
   - Advance Editor
