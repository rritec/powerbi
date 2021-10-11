1. Install DAX Studio, Download software [here](https://daxstudio.org/)
2. Download sample pbix file to follow dax studio tutorial https://github.com/microsoft/powerbi-desktop-samples/blob/main/DAX/Adventure%20Works%20DW%202020.pbix 
3. complet blog https://daxstudio.org/tutorials/writing-dax-queries/
4. Explore online dax examples https://dax.guide/

## Write Dax Queries by comparing SQL Queries

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

## Exercise: Create a tabe in powerBI using below dax query
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

