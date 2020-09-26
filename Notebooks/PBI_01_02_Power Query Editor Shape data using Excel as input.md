
# Power Query Editor
- It is also known as `Power Query`


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
https://docs.microsoft.com/en-us/power-bi/desktop-add-custom-column

https://docs.microsoft.com/en-us/powerquery-m/power-query-m-function-reference


```python

```
