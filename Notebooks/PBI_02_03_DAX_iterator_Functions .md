# Use aggregation iterator functions

- Each single-column summarization function has its equivalent iterator function.
- Example sum > sumx, min > minx, max > maxx, rank >rankx, count>countX, counta > countaX ..etc
- All scenarios of sum/min/max ..etc can also achivable using respective sumX/minX/maxX.... etc, however first priority goes to sum/min/max ..etc



## What is the difference between SUM() Vs SUMX()?
   - https://exceleratorbi.com.au/use-sum-vs-sumx/   
   - SUM() operates over a **single column** and has no awareness of individual rows in the column (no row by row evaluation).
   - SUMX() can operate on **multiple columns** in a table and can complete row by row evaluation in those columns.
   - SUMX() vs SUM(): Which One Should I Use?
      - Which you use really depends on your personal preference and the **structure of your data**.
      - In below example what we should use ?
      
      | product  | Quantity | Unit Price |        
      | ------------- | ------------- | -------- |        
      | Product 1 |	2	| 100 |        
      | Product 2 |	4	| 120 |        
      | Product 3 |	8 |	130 |
      
      - Answer is : Sumx
      - In below example what we should use ?
      
      
      | product  | Total Price |        
      | ------------- | -------- |        
      | Product 1 |	200 |        
      | Product 2 |	480 |        
      | Product 3 |	1040|
      
      
      - Answer is sum

   ### Process Steps:
   ----
   -  From SQL Server **Adventureworksdw2012** > Import **FactInternetSales** and **Customer** Table
   -  Observe the **Model** Relationship based on **customerkey** automatically created
   -  Creat a table visualization with three columns **English Education**,**TotalProductCost**,**SalesAmount**
   -  ![image](https://user-images.githubusercontent.com/20516321/168948738-e6c7985b-f620-4e4d-aeba-bf0529b7ea61.png)

   -  Create **Margin** Measure using below formula
   
           Margin = sumx(FactInternetSales,FactInternetSales[SalesAmount]-FactInternetSales[TotalProductCost])
   -  Create **TotalMargin** Measure using below formula
   
            TotalMargin = sumx(all(FactInternetSales),FactInternetSales[SalesAmount]-FactInternetSales[TotalProductCost])
   -  Create **% Margin Contribution** Measure using below formula
   
            % Margin Contribution = DIVIDE([Margin],[TotalMargin])
   -  Select **% Margin** > Change format as **Percentage**
   -  For more information Follow below blog and Develop below report
   - [Reference](https://radacad.com/sum-vs-sumx-what-is-the-difference-of-the-two-dax-functions-in-power-bi)
      ![image](https://user-images.githubusercontent.com/20516321/117744290-065a1380-b226-11eb-971f-87b9c80729a0.png)

## Calculate ranks

```sql

select e.*,
sum(sal) over ( partition by deptno),
rank() over(order by sal) as rank1,
dense_rank() over(order by sal) as denserank,
rank() over (partition by deptno order by sal desc) as p_based_on_deptno_rank
from emp as e
order by deptno
```

- The RANKX DAX function is a special iterator function you can use to calculate ranks. Its syntax is as follows:
```RANKX(<table>, <expression>[, <value>[, <order>[, <ties>]]])```
- Ref Help [doc](https://docs.microsoft.com/en-us/dax/rankx-function-dax)
- Similar to all iterator functions, you must pass in a table and an expression. Optionally, you can pass in a rank value to find the order direction or to help you determine how to handle ranks when values are tied.

## Order direction
- Order direction is either ascending or descending.
- When ranking something favorable, like revenue values, you're likely to use descending order so that the highest revenue will be ranked first. 
- When ranking something unfavorable, like customer complaints, you might use ascending order so that the lowest number of complaints will be ranked first. 
- When you don't pass in an order argument, the function will use descending order.

## Handle ties
- You can handle ties by skipping rank values or using dense ranking, which uses the next rank value after a tie. 
- When you don't pass in a ties argument, the function will use skipped. 
- You'll have an opportunity to work with an example of each tie argument in subsequent sections.

## Create ranking measures
- Download [file](https://github.com/rritec/powerbi/raw/master/Labdata/Adventure%20Works%20DW%202020%20M05.pbix)
- Open file 
- Add the following measure 

  ```Product Quantity Rank = RANKX(ALL('Product'[Product]),[Quantity])```

- Add the Product Quantity Rank measure to the table visual that is found on Page 2 of the report. The table visual groups bike products and displays quantity, which orders products by descending quantity.
- The RANKX function iterates over a table that is returned by the ALL DAX function. The ALL function is used to return all rows in a model table or values in one or more columns, and it ignores all filters. Therefore, in this case, it returns a table that consists of all Product column values in the Product table. The RANKX function must use the ALL function because the table visual will group by product (which is a filter on the Product table).
- In the table visual, notice that two products tie for tenth place and that the next product's rank is 12. This visual is an example of using the Skipped ties argument.
- Bike Sales table visual with columns: Product, Quantity, and Rank, ordered by Quantity descending.
![image](https://user-images.githubusercontent.com/20516321/110742032-a7931080-825b-11eb-9bd3-40a885fb958e.png)

- Your next task is to enter the following logic to modify the Product Quantity Rank measure definition to use dense ranking:

  ``` Product Quantity Rank =RANKX(ALL('Product'[Product]),[Quantity],,,DENSE)```

- In the table visual, notice that a skipped ranking no longer exists. After the two products that tie for tenth place, the next ranking is 11.
- Bike Sales table visual with columns: Product, Quantity, and Rank, ordered by Quantity descending, but with dense ranking.
    ![image](https://user-images.githubusercontent.com/20516321/110742454-67805d80-825c-11eb-82e1-752da4ebc908.png)

- Notice that the table visual total for the Product Quantity Rank is one (1). The reason is because the total for all products is ranked.
- An image shows the Product Quantity Rank total is 1.
- It's not appropriate to rank total products, so you will now use the following logic to modify the measure definition to return BLANK, unless a single product is filtered:
  ```Product Quantity Rank = IF(HASONEVALUE('Product'[Product]),RANKX(ALL('Product'[Product]),[Quantity],,,DENSE))```
- An image shows the Product Quantity Rank total is BLANK.
  ![image](https://user-images.githubusercontent.com/20516321/110742868-20df3300-825d-11eb-888b-5f11d71d8857.png)

- Notice that the total Product Quantity Rank is now BLANK, which was achieved by using the HASONEVALUE DAX function to test whether the Product column in the Product table has a single value in filter context. It's the case for each product group, but not for the total, which represents all products.

**Home work:** [Top N dynamic selections](https://github.com/rritec/powerbi/blob/566b75a3a5850984fc9a9d9549104ce3dd70befe/Notebooks/Interview%20Questions/Top%20N%20Dynmic%20Selecton%20using%20what%20if%20parameter.md)

## Count Vs counta & count vs countx & counta vs countax
  - Enter below data and create a table

      | Employee Name | Date  | Holiday Flag | phone |        
      | ------------- | ------------- | ------------- | -------- |        
      | Ram | 01-Jan-2016 |	False	| 9573707079 |        
      | John | 02-Jan-2017 |	True	|  |        
      | Nancy | 01-Jan-2019 |	False |	1234567890 |

  - Make sure datatypes are Employee Name --> Text, Date --> Date , Holiday Flag --> Bool, Phone --> Whole Number
  - Can you count Date column using count and counta function?
      - yes
  - can you count bool column with count function?
      - No
  - Can you count bool column with counta?
      - Yes

  - count number of rows when holiday flag is *False*
      - *Hint*: use below formula inside the measure 
      - COUNTAX(FILTER(count_understanding,count_understanding[Holiday Flag]=FALSE()),count_understanding[Holiday Flag])
- Try below example
![image](https://github.com/rritec/powerbi/assets/20516321/46b43888-40e8-4396-bf30-dfe9e49fc504)




