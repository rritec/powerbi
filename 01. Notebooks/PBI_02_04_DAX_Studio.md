## About

- DAX Studio is a tool to write, execute, and analyze DAX queries in Power BI Desktop, Power Pivot for Excel, and Analysis Services Tabular.

## Setup environment 
1. Download DAX Studio Software [here](https://daxstudio.org/)
2. Double click on DAX STUDIO > Install it.
3. Download sample pbix file to follow dax studio tutorial https://github.com/microsoft/powerbi-desktop-samples/raw/main/DAX/Adventure%20Works%20DW%202020.pbix 
4. Open the above Power BI file
5. Go to Power BI Desktop > External Tools > Click on DAX Studio
## Tutorial 
7. Follow blog https://daxstudio.org/tutorials/writing-dax-queries/
### How to query a table of data?
Syntax: Evaluate \<Table Expression\>
       
        EVALUATE customer
More Examples:

        EVALUATE CALENDAR(date(2021,10,01),date(2021,10,05))
        EVALUATE FILTER(Customer,Customer[City]="Concord") 
        EVALUATE CALCULATETABLE(Customer,Customer[City]="Concord")
### How to query a table or column of data?
Syntax: VALUES\<tablename or columnname\>
        
        EVALUATE VALUES(Customer)
        EVALUATE VALUES(Customer[City])
        EVALUATE CALCULATETABLE(VALUES(Customer[City]),LEFT(Customer[City],1)="C")
        EVALUATE FILTER(VALUES(Customer[City]),LEFT(Customer[City],1)="C")

### How to sort the data?
Syntax: ORDER BY \<column names\> ASC/DESC
        
        EVALUATE CALCULATETABLE( VALUES ( Customer[City] ), LEFT ( Customer[City], 1 ) = "R" ) ORDER BY Customer[City]
        
### Returning a single value?

        
        EVALUATE { SUM ( Sales[Sales Amount] ) }
               
 ### Selecting columns from multiple tables?

        
        EVALUATE
        SUMMARIZECOLUMNS (
            Product[Color],
            Reseller[Business Type],
            FILTER ( ALL ( Product[List Price] ), Product[List Price] > 150.00 ),
            TREATAS ( { “Accessories”, “Bikes” }, ‘Product’[Category] ),
            “Total Sales”, SUM ( Sales[Sales Amount] )
        )
        
### Multiple Resultsets?

        
        EVALUATE Customer
        EVALUATE Product       

### Using Parameters in Queries?

        
        EVALUATE FILTER ( 'Product', 'Product'[Color] = @color_name )
        

### Write Dax Queries by comparing SQL Queries

// select * from Customer
//EVALUATE Customer

// select city from customer
//EVALUATE VALUES(Customer[City])

// select * from customer where city ="redmond"
//EVALUATE CALCULATETABLE ( Customer, Customer[City] = "Redmond" )

// select city  from customer where city like "R%"
//EVALUATE CALCULATETABLE(VALUES(Customer[City]),left(Customer[City],1)="R")

// select *  from customer where city like "R%"
//EVALUATE CALCULATETABLE(Customer,left(Customer[City],2)="Ro")

// select city  from customer where city like "R%" order by city desc
//EVALUATE CALCULATETABLE(VALUES(Customer[City]),left(Customer[City],1)="R") ORDER BY Customer[City] desc

![image](https://user-images.githubusercontent.com/20516321/169445380-cf011b56-3c7c-485f-bdc4-ced3857f1dc3.png)


### Exercise: Create a tabe in powerBI using below dax query
1. In DAX studio write below Dax query, run it  and understand result. 

        EVALUATE SUMMARIZECOLUMNS (
              Product[Color],
              Reseller[Business Type],
              FILTER ( ALL ( Product[List Price] ), Product[List Price] > 150.00 ),
              TREATAS ( { "Accessories", "Bikes" }, 'Product'[Category] ),
              "Total Sales", SUM ( Sales[Sales Amount] )
          )
2. Once we are happy with result then create table inside PBI
3. open PBI Desltop > data page
4. click on Dax Table, write below dax formula

        test_table_name =
          SUMMARIZECOLUMNS (
              Product[Color],
              Reseller[Business Type],
              FILTER ( ALL ( Product[List Price] ), Product[List Price] > 150.00 ),
              TREATAS ( { "Accessories", "Bikes" }, 'Product'[Category] ),
              "Total Sales", SUM ( Sales[Sales Amount] )
          )
5. Observe result

 ### More Examples

Explore online dax examples https://dax.guide/
Compare SQL to DAX Query examples  https://www.sqlbi.com/articles/from-sql-to-dax-projection/

