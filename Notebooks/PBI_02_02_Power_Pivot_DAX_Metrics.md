
# Power Pivot

## Data Analysis Expressions (DAX):
1. Data Analysis Expressions (DAX) is a library of functions and operators that can be combined to build formulas and expressions in 
    - Power BI Desktop
    - Azure Analysis Services
    - SQL Server Analysis Services
    - Power Pivot in Excel data models.
1. DAX formulas include functions, operators, and values to perform advanced calculations and queries on data in related tables and columns in tabular data models.


https://docs.microsoft.com/en-us/dax/

https://docs.microsoft.com/en-us/learn/paths/dax-power-bi/

# DAX Main Types are

## Date and time functions


### CALENDAR
1. Open PBI Desktop
1. Click on **Model** Menu bar
1. Click on New Table
1. Provide DAX formula as **Calendar = CALENDAR (DATE (2019, 1, 1), DATE (2020, 12, 31))**
1. Develop Table Report and observe output.

1. Also explore DATE,EOMONTH, DATEDIFF, TODAY

## Time-intelligence functions

### SAMEPERIODLASTYEAR
- Refer next lesson 

## Filter functions

### CALCULATE
- Refer next lesson 

## Information functions
- username()
- userprincipalname()
- isblank
- iserror
- contains
- ...etc

## Logical functions
- and
- or
- if
- ...etc

## Math and Trig functions
- sin
- cos
- log
- exp
- ..etc

## Statistical functions
- AVERAGE
- COUNT
- MAX
- MIN
- ... etc

## Exercise 1: Using Variables to improve performance
- Any calculation, we are using twice are more better to store the calculation result in variable and use the variable where ever needed.
- Open Labdata/Adventure Works DW 2020 M02.pbix file
- Observe Calculation inside **Sales** table **Revenue YoY %**
- The last year sales, calculating two times right .
- Develop one mesure with the name of **Revenue YOY % using Var** with below formula

    ```
    Revenue YoY %_var = 
    VAR LYSales = CALCULATE([Revenue], SAMEPERIODLASTYEAR('Date'[Date]))
    RETURN
    DIVIDE([Revenue] - LYSales, LYSales) 
    ```
- Develop report as shown below
    - ![image](https://user-images.githubusercontent.com/20516321/111411593-da785100-8700-11eb-94d7-c8e177cf87b9.png)

## Exercise 2: Duplicate Table
- Open [Adventure Works DW 2020 M03](https://github.com/rritec/powerbi/raw/master/Labdata/Adventure%20Works%20DW%202020%20M03.pbix)
- In the Data view > Click on New Table > type below formula 

    ```
    Ship Date = 'Date'
    ```
- To complete the design of the Ship Date table, you can:
    - Rename the following columns:
        - **Date** as **Ship Date**
        - **Fiscal Year** as **Ship Fiscal Year**
        - **Fiscal Quarter** as **Ship Fiscal Quarter**
        - **Month** as **Ship Month**
        - **Full Date** as **Ship Full Date**
    - Sort the **Ship Full Date** column by the **Ship Date** column.
    - Sort the **Ship Month** column by the **MonthKey** column.
    - Hide the **MonthKey** column.
    - Create a hierarchy named Fiscal with the following levels:
        - Ship Fiscal Year
        - Ship Fiscal Quarter
        - Ship Month
        - Ship Full Date
    - Mark the **Ship Date** table as a date table by using the Ship Date column.

## Exercise 3: Can you populate dates of india financial year
- The financial year of India begins from April 1 of a calendar year and ends on March 31 of the next calendar year
- In above PBIX file, develop a table report to understand range of dates

  ![image](https://user-images.githubusercontent.com/20516321/111573915-72de0680-87d1-11eb-8895-158a5d895da2.png)

- In the Data view > Click on New Table > type below formula 

    ```
    India Fin Dates =  CALENDARAUTO(3)
    ```
 - Using **India Fin Dates** Table **Date** Column  develop below report and understand how the Calendar Auto working.

   ![image](https://user-images.githubusercontent.com/20516321/111574107-d831f780-87d1-11eb-83ca-9b1254d9e1ff.png)

 - Read the [doc](https://docs.microsoft.com/en-us/dax/calendarauto-function-dax)


## calculated columns Vs measures

- DAX beginners often experience a degree of confusion about calculated columns and measures. The following section reviews the similarities and differences between both.
    - Regarding similarities between calculated columns and measures, both are:
        - Calculations that you can add to your data model.
        - Defined by using a DAX formula.
        - Referenced in DAX formulas by enclosing their names within square brackets.
    - The areas where calculated columns and measures differ include:
        - **Purpose** - Calculated columns extend a table with a new column, while measures define how to summarize model data.
        - Evaluation - Calculated columns are evaluated by using row context at data refresh time, while measures are evaluated by using filter context at query time. Filter context is introduced in a later module; it's an important topic to understand and master so that you can achieve sophisticated summarizations.
        - Storage - Calculated columns (in Import storage mode tables) store a value for each row in the table, but a measure never stores values in the model.
        - Visual use - Calculated columns (like any column) can be used to filter, group, or summarize (as an implicit measure), whereas measures are designed to summarize.

## Questions
1. Create a table with dates by using given two Dates?
    - Open PBI Desktop
    - Click on **Model** Menu bar
    - Click on New Table
    - Provide DAX formula as **Calendar = CALENDAR (DATE (2019, 1, 1), DATE (2020, 12, 31))**
    - Develop Table Report and observe output.
 1. Difference between USERNAME() Vs USERPRINCIPALNAME()?
    - https://docs.microsoft.com/en-us/dax/username-function-dax
    - https://docs.microsoft.com/en-us/dax/userprincipalname-function-dax
    - In PowerBI Desktop
        - ![image](https://user-images.githubusercontent.com/20516321/109728973-34dfc080-7bdd-11eb-8dbb-ad4fd8316da4.png)
    - In Power BI Service
        - ![image](https://user-images.githubusercontent.com/20516321/109729142-740e1180-7bdd-11eb-9ec5-25db46bfd2cf.png)
        
 1. What is User Principal Name?
    - User Principal Name (UPN) is the name of a system user in an email address format.
    - A UPN (for example: john.doe@domain.com) consists of the user name (logon name), separator (the @ symbol), and domain name (UPN suffix)
 1. How many years survived by Mahatma Gandhi? 
    - We know Gandhi Born on **October 2, 1869**, and Died on **January 30, 1948**
    - Read help document and find out no of years survived by Gandhi 
    - https://docs.microsoft.com/en-us/dax/datediff-function-dax
 1.  What is the difference between SUM() Vs SUMX()?
     - https://exceleratorbi.com.au/use-sum-vs-sumx/
     - https://radacad.com/sum-vs-sumx-what-is-the-difference-of-the-two-dax-functions-in-power-bi
     - SUM() operates over a single column and has no awareness of individual rows in the column (no row by row evaluation).
     - SUMX() can operate on multiple columns in a table and can complete row by row evaluation in those columns.
 1. Count Vs counta & count vs countx & counta vs countax
    - Enter below data and create a table

        | Date  | Holiday Flag | phone |        
        | ------------- | ------------- | -------- |        
        | 01-Jan-2016 |	False	| 9573707079 |        
        | 02-Jan-207 |	True	|  |        
        | 01-Jan-2019 |	False |	1234567890 |
        
    - Make sure datatypes are Date --> Date , Holiday Flag --> Bool, Phone --> Whole Number
    - Can you count Date column using count and counta function?
        - yes
    - can you count bool column with count function?
        - No
    - Can you count bool column with counta?
        - Yes
   
    - count number of rows when holiday flag is *False*
        - *Hint*: use below formula inside the measure 
        - COUNTAX(FILTER(count_understanding,count_understanding[Holiday Flag]=FALSE()),count_understanding[Holiday Flag])    
1. Calculated columns Vs measures

    - DAX beginners often experience a degree of confusion about calculated columns and measures. The following section reviews the similarities and differences between both.
        - Regarding similarities between calculated columns and measures, both are:
            - Calculations that you can add to your data model.
            - Defined by using a DAX formula.
            - Referenced in DAX formulas by enclosing their names within square brackets.
        - The areas where calculated columns and measures differ include:
            - **Purpose** - Calculated columns extend a table with a new column, while measures define how to summarize model data.
            - **Evaluation** - Calculated columns are evaluated by using row context at data refresh time, while measures are evaluated by using filter context at query time. Filter context is introduced in a later module; it's an important topic to understand and master so that you can achieve sophisticated summarizations.
            - **Storage** - Calculated columns (in Import storage mode tables) store a value for each row in the table, but a measure never stores values in the model.
            - **Visual use** - Calculated columns (like any column) can be used to filter, group, or summarize (as an implicit measure), whereas measures are designed to summarize.


 


```python

```
