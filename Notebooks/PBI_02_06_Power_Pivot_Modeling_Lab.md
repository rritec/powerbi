
# `Power BI Desktop Modelling`
- It is also knon as **Power Pivot**
- In power pivot mainly we will do
    - Relation Ships(Among Queries)
    - DAX Formulas

## SCENARIO
VanArsdel is a company that manufactures and sells sporting goods. The company has offices in the United States (US) and several other countries. Its sales comprise of US sales and International sales. VanArsdel’s sales come from its owned manufactured products, as well as other manufacturers’ products.

You have successfully brought the US sales data from the Access database and the International sales data from a collection of CSV files to Power BI Desktop. 

Before you can start analyzing your data, you need to manage the table relationships within your data model and create new ones if necessary. To do so, you might need to create calculated columns or calculated tables for the relationships to be based on.
Once you have all the relationships created, you can create visualizations and start to analyze the data. However, you need to create additional measures to perform more advanced analysis with your data, which includes:

- Comparing current year YTD sales and last year YTD sales.
- Comparing sales of VanArsdel's manufactured goods to other manufacturers.


## LAB OVERVIEW

In this lab, you will create 
    - calculated columns 
    - calculated tables
    - create table relationships in your data model based on the calculated columns and tables you created. 
In addition, you will write several DAX expressions to create measures to be used to analyze VanArsdel’s sales data. Specifically, you will create the following measures:
1. `Total Sales:` calculates the total sales.
2. `LY Sales:` calculates last year sales.
3. `Sales Var:` calculates sales variance between this year and last year sales.
4. `Sales Var %:` calculates sales variance between this year and last year sales in percentage.
5. `YTD Sales:` calculates YTD sales.
6. `LY YTD Sales:` calculates last year YTD sales.
7. `YTD Sales Var:` calculates sales variance between this year and last year YTD sales.
8. `YTD Sales Var %:` calculates sales variance between this year and last year YTD sales in percentage.
9. `Total VanArsdel Sales:` calculates sales for VanArsdel manufactured goods.
10. `% Sales Market Share:` calculates the percentage of VanArsdel manufactured goods from the total sales.



## WHAT YOU’LL NEED
The “Lab 2 - Starting.pbix” file

## Exercise 1- Manage Table Relationships
Power BI Desktop has automatically detected and created table relationships. So the first step is to ensure all the relationships are properly created, and if not, create them yourselves.


1. Open the `Lab2 - Starting.pbix` file from our `Labdata/Lab2 folder`.
2. In the navigation pane on the left, click `Model`

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0000.png?raw=true).
    
3. Notice that there is a **many to one** relationship from the `ProductID` column on the `Sales` table to the `ProductID` column on the `Products` table.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0002.png?raw=true)
    
4. Notice that there is a **many to one** relationship from the `ManufacturerID` column on the `Products` table to the `ManufacturerID` column on the `Manufacturers` table.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0004.png?raw=true)

5. Drag the `Date` column on the `Sales` table to the `Date` column on the `Date` table.
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0003.png?raw=true)
    
6. Now you want to create a relationship between the `Sales` table and the `Locations` table. First, you merge the `Country` and `Zip` columns in both `Sales` and `Locations` table as a new column, `CountryZip`. Then, you create a relationship on the `CountryZip` column for both tables.
    - In the `navigation pane` on the left, click `Data`
    
        ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0005.png?raw=true).
        
    - In the navigation pane on the right, click `Location`.
    - On the Modeling ribbon, click New Column.
    - In the formula bar for the new column, type `CountryZip = Locations[Country] & ", " & Locations[Zip]`, and press `Enter`.
        
        ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0008.png?raw=true)
        
    - In the navigation pane on the right, click Sales.
    - On the Modeling ribbon, click New Column.
    - In the formula bar for the new column, type `CountryZip = Sales[Country Name] & ", " & Sales[Zip]`, and press `Enter`.
        
        ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0006.png?raw=true)
        
    - In the navigation pane on the left, click **Model**.
    - Drag the **CountryZip** column on the **Sales** table to the **CountryZip** column on the **Locations** table.
    
        ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0007.png?raw=true)
        
16. Click **Save**, to save the Power BI file.

## Exercise 2- Last Year Comparison

- You want to know how much sales (revenue) in total does the VanArsdel have and to compare this with the figure from the same period last year. You need to create several calculated measures to help with this comparison. To do so, in either the Report view or the Data view, right-click the Sales table, click New Measure, and type in the corresponding DAX formulas for the measure you want to create. This will create the measures with the Home Table properties set to the Sales table.
- Specifically, you will create the following measures:
    - `Total Sales:` calculates the total sales. Format this measure as Currency. (Hint: Check out the SUM function).
    - `LY Sales:` calculates last year sales. Format this measure as Currency. (Hint: You might find the CALCULATE and SAMEPERIODLASTYEAR function useful).
    - `Sales Var:` calculates sales variance between this year and last year sales. Format this measure as Currency. (Hint: This is simply the difference between Total Sales and LY Sales).
    - `Sales Var %:` calculates sales variance between this year and last year sales in percentage. Format this measure as Percentage. (Hint: This is simply the percentage of Sales Var from LY Sales. You might find the DIVIDE function useful).

1. In the navigation pane on the left, click `Data`
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0005.png?raw=true).
2. In the navigation pane on the right, click `Sales`.
3. On the Modeling ribbon, click `New Measure`.
4. In the formula bar for the new measure, type `Total Sales = SUM(Sales[Revenue])`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0009.png?raw=true)

5. On the `Modeling` ribbon, click `Format`, click `Currency`, and click `Currency general`.
6. On the Modeling ribbon, click New Measure.
7. In the formula bar for the new measure, type `LY Sales = CALCULATE([Total Sales],SAMEPERIODLASTYEAR(‘Date’[Date]))`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0010.png?raw=true)

8. On the `Modeling` ribbon, click `Format`, click `Currency`, and click `Currency general`.
9. On the `Modeling` ribbon, click `New Measure`.
10. In the formula bar for the new measure, type `Sales Var = [Total Sales] - [LY Sales]`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0011.png?raw=true)

11. On the `Modeling` ribbon, click `Format`, click `Currency`, and click `Currency general`.
12. On the `Modeling` ribbon, click `New Measure`.
13. In the formula bar for the `new measure`, type `Sales Var % = DIVIDE([Sales Var],[LY Sales]) `, and press `Enter`.

    
14. On the `Modeling` ribbon, click `Format`, and click `Percentage`.
15. Click `Save`, to save the Power BI file.
16. Develop below report and understand results

    ![image](https://user-images.githubusercontent.com/20516321/112080270-a8a33680-8ba7-11eb-8346-299e0f052cb2.png)


`Home Work:`
- Total Units: Total Units = SUM(Sales[Units])
- LY Total Units: LY Total Units = CALCULATE([Total Units],SAMEPERIODLASTYEAR(‘Date’[Date])
- Total Units Var: Total Units Var = [Total Units] - [LY Total Units]
- Total Units Var %: Total Units Var % = DIVIDE([Total Units Var],[LY Total Units])


## Exercise 3- Year to Date
- Year-to-date (YTD) is a period starting from the beginning of the current year and continuing up to the present date. You want to calculate the YTD sales and compare this with the figure from the same period last year. Specifically, you will create the following measures:
    - YTD Sales: calculates the YTD sales. Format this measure as Currency. (Hint: Check out the TOTALYTD function).
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0013.png?raw=true)
    
    - LY YTD Sales: calculates last year YTD sales. Format this measure as Currency. (Hint: You might find the CALCULATE and SAMEPERIODLASTYEAR function useful).
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0014.png?raw=true)
    
    - YTD Sales Var: calculates sales variance between this year and last year YTD sales. Format this measure as Currency. (Hint: This is simply the difference between YTD Sales and LY YTD Sales).
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0015.png?raw=true)
    
    - YTD Sales Var %: calculates sales variance between this year and last year YTD sales in percentage. Format this measure as Percentage. (Hint: This is simply the percentage of YTD Sales Var from LY YTD Sales. You might find the DIVIDE function useful).
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0017.png?raw=true)
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0110.png?raw=true)
    

`Home Work:`
1. YTD Total Units: YTD Total Units = TOTALYTD([Total Units],‘Date’[Date])
2. LY YTD Total Units: LY YTD Total Units = CALCULATE([YTD Total Units],SAMEPERIODLASTYEAR(‘Date’[Date]))
3. YTD Total Units Var: YTD Total Units Var = [YTD Total Units]- [LY YTD Total Units]
4. YTD Total Units Var %: YTD Total Units Var % = DIVIDE([YTD Total Units Var],[LY YTD Total Units])

## Exercise 4- Market Share

- VanArsdel sales comprise of products manufactured by VanArsdel and other companies. You want to know how much of these sales are VanArsdel’s own manufactured products. You decide to show this share in numbers and %. Specifically, you will create the following measures:
- Total VanArsdel Sales: calculates sales where the products manufacturer is VanArsdel. Format this measure as Currency. (Hint: Use the CALCULATE function and filter by Manufacturer).
- % Sales Market Share: calculates the percentage of sales of VanArsdel manufactured products from the total sales. Format this measure as Percentage.

1. In the navigation pane on the left, click `Data`.
2. In the navigation pane on the right, click `Sales`.
3. On the `Modeling` ribbon, click `New Measure`.
4. In the formula bar for the new measure, type `Total VanArsdel Sales = CALCULATE([Total Sales],Manufacturer[Manufacturer]="VanArsdel")`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0019.png?raw=true)

5. On the `Modeling` ribbon, click `New Measure`.
6. In the formula bar for the new measure, type `% Sales Market Share = IF([Total VanArsdel Sales]=0,0,DIVIDE([Total VanArsdel Sales],[Total Sales],0))`, and press `Enter`.

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0018.png?raw=true)

7. On the `Modeling` ribbon, click `Format`, and click `Percentage`.
8. Click `Save`, to save the Power BI file.

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0111.png?raw=true)

`Home Work:`
- Total VanArsdel Units: Total VanArsdel Units = CALCULATE([Total Units],Manufacturers[Manufacturer]=“VanArsdel”)
- % Units Market Share: % Units Market Share = IF([Total VanArsdel Units]=0,0,DIVIDE([Total VanArsdel Units],[Total Units],0))


## Exercise 5- Optimize the Data Model

1. Now that you have the table relationships defined and the measures created, you want to optimize the data model before you create the visualizations.
1. If it is not already open, open the Lab 2 - Starting.pbix file.
1. Ensure both the **International Sales** and **Country Population** table are hidden from the report view using the following steps.
1. In the navigation pane on the left, click `Data`.
1. In the navigation pane on the right, click the ellipses (...) adjacent to - `International Sales` and click `Hide in report view`.
1. In the navigation pane on the right, click the ellipses (...) adjacent to `Country Population` and click Hide in report view.
1. Hide the following fields on the `Date` table from the report view:
    - MonthNo
    - MonthID
    - Month
        - In the navigation pane on the right, click `Date`, click the ellipses (...) adjacent to `MonthNo` and click `Hide in report view`.
        - In the navigation pane on the right, click Date, click the ellipses(...) adjacent to `MonthID` and click `Hide in report view`.
        - In the navigation pane on the right, click Date, click the ellipses(...) adjacent to `Month` and click `Hide in report view`.
5. Sort the MonthName column by the MonthNo column using the following steps.
    - Click the `MonthName` column and, on the Modeling ribbon, click `Sort by Column`, and click `MonthNo`.
9. Hide the `CountryZip` field on the `Location` table and the `ManufacturerID` field on the `Manufacturer` table from the report view using the following steps.
    - In the navigation pane on the right, click Location, click the ellipses adjacent to CountryZip and click Hide in report view.
    - In the navigation pane on the right, click Manufacturer, click the ellipses adjacent to ManufacturerID and click Hide in report view.
10. Hide the following fields on the **Products** table from the report view.
    - ProductID
    - ManufacturerID
    - Manufacturer
        - In the navigation pane on the right, click Products, click the ellipses(...) adjacent to ProductID and click Hide in report view.
        - Click the ellipses adjacent to ManufacturerID and click Hide in report view.
        - Click the ellipses adjacent to Manufacturer and click Hide in report view.
8. Hide the following fields on the **Sales** table from the report view.
    - ProductID
    - Date
    - Zip
    - Units
    - Revenue
    - Country Name
    - CountryZip
        - In the navigation pane on the right, click Sales, 
        - Click the ellipses adjacent to `ProductID` and click `Hide in report view`.
        - Click the ellipses adjacent to `Date` and click `Hide in report view`.
        - Click the ellipses adjacent to `Zip` and click `Hide in report view`.
        - Click the ellipses adjacent to `Units` and click `Hide in report view`.
        - Click the ellipses adjacent to `Revenue` and click `Hide in report view`.
        - Click the ellipses adjacent to `Country Name` and click `Hide in report view`.
        - Click the ellipses adjacent to `CountryZip` and click `Hide in report view`.
9. Click `Save`, to save the Power BI file.

## Questions
----
1. Can you develop below report
    - ![image](https://user-images.githubusercontent.com/20516321/110577445-ac3ac480-8188-11eb-9afc-a39eb1443a41.png)


```python

```


```python

```
