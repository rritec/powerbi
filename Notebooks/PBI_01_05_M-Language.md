# M-Language

1. Power Query is a Formula Language (Informally known as "M")
2. **M** stands for **Mash-Up**
3. **M** is a case-sensitive language
4. Power Query is a data transformation and data preparation engine. Power Query comes with a graphical interface for getting data from sources and a Power Query Editor for applying transformations. Because the engine is available in many products and services, the destination where the data will be stored depends on where Power Query was used. Using Power Query, you can perform the extract, transform, and load (ETL) processing of data.

![image](https://user-images.githubusercontent.com/20516321/118579120-12584f00-b7ab-11eb-8f40-dee8dd8bfd24.png)

## Reference doc 

https://docs.microsoft.com/en-us/powerquery-m/quick-tour-of-the-power-query-m-formula-language

### Exercise 1: Write Simple M-languge Query

1. Open **Power BI Desktop** > Click on **Get Data** > Click on **Blank Query** > In **Power Query Editor** > Click on **Advanced Editor** > Then copy paste below code

``` F#
let
    x = 1 +1,
    y= x+2,
    z = y+3
in
    z
```
1. Click on done
2. Click on apply and close
3. develop report and observe output
### Exercise 2: Write Simple M-languge Query with spaces in variable name.

1. Replace above code with below code and observe result

``` F#
let
        #"First Name" = "Ram",
        #"Last Name" = "Reddy",
        #"Full Name" = Text.Combine({#"First Name", #"Last Name"})
in
        #"Full Name"
```
            
            
 ### Exercise 3: Call functions in M-language

1. Replace above code with below code and observe result

``` F#
//this is a single line comment
/* This
is 
a
multiline
comment*/

let
   date = #date(2021,04,25),
   year = Date.Year(date)
in
    year
```
### Exercise 4: Real world example

1. Open any one PBIX file and observe M-language code
2. In screenshot below, you can see all basics mentioned so far:
        - **let** and **in** block
        - Variable names matching steps applied in the query
        - Some variable names with hashtag and double quote: #”var name”
        - End of the line characters: **comma**
        - Calling many functions
        ![image](https://user-images.githubusercontent.com/20516321/116349500-c77f9300-a80d-11eb-9559-0d88ac8890b5.png)

### Questions:
---
1. What is the result of below program

```F#
let 
        Sales2007 =  
        [  
            Year = 2007,  
            FirstHalf = 1000,  
            SecondHalf = 1100, 
            Total = FirstHalf + SecondHalf // 2100 
        ], 
        Sales2008 =  
        [  
            Year = 2008,  
            FirstHalf = 1200,  
            SecondHalf = 1300, 
            Total = FirstHalf + SecondHalf // 2500 
        ] 
in 
        Sales2007[Total] + Sales2008[Total]
```

2. What is the result of below program

```F#
let
        SimpleInterest = (p,t,r) => p*t*r/100,
        // Here 
        // p is principal
        // t is time in months
        // r is rate of interest
        rs = SimpleInterest(100,12,2)
in 
        rs
```

3. What is the result of below program

```F#
let
    a =
    [
        x = 1,       
        y = 2,       
        z = x + y    
    ], 
    b = 3             
in 
    a[z] + b         
```

4. What is the result of below program

```F#
let
    a = List.Contains({1, 2, 3, 4, 5}, 3),
    b = List.Contains({1, 2, 3, 4, 5}, 6)
in 
    {a,b}        
```

5. What is the result of below program

```F#
let
        rs = List.Select({1, -3, 4, 9, -2}, each _ > 0)
in 
        rs  
```

6. What is the result of below program

```F#
let
        rs = List.Sum({1, 2, 3})
in 
        rs
```
   


7. What is the result of below program

```F#
let
   student=Table.FromRecords(
    {
        [sno =101,sname="ram",scourse="powerbi",sfee=100],
        [sno =102,sname="nancy",scourse="powerapps",sfee=200],
        [sno =103,sname="john",scourse="powerautomate",sfee=300]
    }
       )
in
    student       

```
8. What is the result of below program

```F#
let
rs = Table.AlternateRows(
    Table.FromRecords({
        [CustomerID = 1, Name = "Bob", Phone = "123-4567"],
        [CustomerID = 2, Name = "Jim", Phone = "987-6543"],
        [CustomerID = 3, Name = "Paul", Phone = "543-7890"]
    }),
    1,1,1
)
in 
        rs       
```
9. What is the result of below program

```F#
let
        rs = Table.FuzzyGroup(
            Table.FromRecords(
                {
                    [EmployeeID = 1, Location = "Seattle"],
                    [EmployeeID = 2, Location = "seattl"],
                    [EmployeeID = 3, Location = "Vancouver"],
                    [EmployeeID = 4, Location = "Seatle"],
                    [EmployeeID = 5, Location = "vancover"],
                    [EmployeeID = 6, Location = "Seattle"],
                    [EmployeeID = 7, Location = "Vancouver"]
                },
                type table [EmployeeID = nullable number, Location = nullable text]
            ),
            "Location",
            {"Count", each Table.RowCount(_)},
            [IgnoreCase = true, IgnoreSpace = true]
        )
in 
        rs       
```

10. What is the result of below program

```F#
let
    startdate=DateTime.From(#date(2022, 1, 1)),
    enddate=DateTime.LocalNow(),
    numberofdays=Duration.Days(enddate-startdate),
    Dates = List.DateTimes(startdate, numberofdays+1, #duration(1,0,0,0)),
    #"Converted to Table" = Table.FromList(Dates, Splitter.SplitByNothing(), null, null, ExtraValues.Error),
    #"Renamed Columns" = Table.RenameColumns(#"Converted to Table",{{"Column1", "Date"}}),
    #"Changed Type" = Table.TransformColumnTypes(#"Renamed Columns",{{"Date", type datetime}}),
    #"Added Custom" = Table.AddColumn(#"Changed Type", "year", each Date.Year([Date])),
    #"Changed Type1" = Table.TransformColumnTypes(#"Added Custom",{{"year", Int64.Type}}),
    #"Added Custom1" = Table.AddColumn(#"Changed Type1", "monthnumber", each Date.Month([Date])),
    #"Added Custom2" = Table.AddColumn(#"Added Custom1", "Monthname", each Date.MonthName([Date])),
    #"Changed Type2" = Table.TransformColumnTypes(#"Added Custom2",{{"monthnumber", Int64.Type}, {"Monthname", type text}}),
    #"Added Custom3" = Table.AddColumn(#"Changed Type2", "daynumber", each Date.Day([Date])),
    #"Added Custom4" = Table.AddColumn(#"Added Custom3", "weeknumber", each Date.WeekOfYear([Date])),
    #"Changed Type4" = Table.TransformColumnTypes(#"Added Custom4",{{"weeknumber", Int64.Type}}),
    #"Added Custom5" = Table.AddColumn(#"Changed Type4", "DayName", each Date.DayOfWeekName([Date],"en-US"))
    
in
     #"Added Custom5"     
```
 
