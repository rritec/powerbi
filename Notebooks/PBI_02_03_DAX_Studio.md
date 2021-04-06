1. Install DAX Stdio, Download software [here](https://daxstudio.org/)
2. https://github.com/microsoft/powerbi-desktop-samples/tree/main/DAX
3. complet blog https://daxstudio.org/tutorials/writing-dax-queries/

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

