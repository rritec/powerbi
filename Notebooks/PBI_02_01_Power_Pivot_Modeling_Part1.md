
# Power Pivot
  - It is useful to do two activities  
    1. Modeling
        - Relation ship(Among Tables) Vs Join(Among Queries)
        - Cardinality
          - One to One
          - One to Many
          - **Many to One**(Default)
          - Many to Many
        - Cross Filter Directions
          - **Single**(Default)
          - Both
        - Active Vs Inactive Relationships       
    2. DAX Calculations  
## Exercise 1: Create Two tables using Enter Data Method
1. When you import multiple tables, chances are you'll do some analysis using data from all those tables. Relationships between those tables are necessary to accurately calculate results and display the correct information in your reports.
2. Power BI Desktop makes creating those relationships easy. In fact, in most cases you won’t have to do anything, the autodetect feature does it for you based on common column names and data.
3. The first table, **ProjectHours**, is a record of work tickets that record the number of hours a person has worked on a particular project. 
4. Open **Power BI Desktop** > In the toolbar click on **Enter Data** > Provide **Table Name** as **ProjectHours** > copy below data and paste into workspace

    | **Ticket** | **SubmittedBy** | **Hours** | **Project** | **DateSubmit** |
    | ---:|:--- | ---:|:--- | ---:|
    | 1001 |Brewer, Alan |22 |Blue |1/1/2013 |
    | 1002 |Brewer, Alan |26 |Red |2/1/2013 |
    | 1003 |Ito, Shu |34 |Yellow |12/4/2012 |
    | 1004 |Brewer, Alan |13 |Orange |1/2/2012 |
    | 1005 |Bowen, Eli |29 |Purple |10/1/2013 |
    | 1006 |Bento, Nuno |35 |Green |2/1/2013 |
    | 1007 |Hamilton, David |10 |Yellow |10/1/2013 |
    | 1008 |Han, Mu |28 |Orange |1/2/2012 |
    | 1009 |Ito, Shu |22 |Purple |2/1/2013 |
    | 1010 |Bowen, Eli |28 |Green |10/1/2013 |
    | 1011 |Bowen, Eli |9 |Blue |10/15/2013 |

5. This second table, **CompanyProject**, is a list of projects with an assigned priority: A, B, or C. Create this table also simillar to above table.

    | **ProjName** | **Priority** |
    | --- | --- |
    | Blue |A |
    | Red |B |
    | Green |C |
    | Yellow |C |
    | Purple |B |
    | Orange |C |
6. Notice that each table has a **project** column. Each is named slightly different, but the values look like they’re the same.
## Exercise 2: Number of hours submitted by project priority without relationship
1. Select **Priority** and **Hours** from the **Fields** pane.  
2. If we look at our table in the report canvas, you’ll see the number of hours is 256 for each project, which is also the total. Clearly this number isn’t correct. Why? It’s because we can’t calculate a sum total of values from one table (**Hours** in the **Project** table), sliced by values in another table (**Priority** in the **CompanyProject** table) without a relationship between these two tables.
## Exercise 3: Number of hours submitted by project priority with relationship
7. Go to model and create relation using **ProjName** and **project** columns
8. Come to report observe the data.
## Exercise 4: Add one more table to above Model

7. Click on **Enter Data** > create below table

  **EmployeeRole**

  | **Employee** | **Role** |
  | --- | --- |
  | Bento, Nuno |Project Manager |
  | Bowen, Eli |Project Lead |
  | Brewer, Alan |Project Manager |
  | Hamilton, David |Project Lead |
  | Han, Mu |Project Lead |
  | Ito, Shu |Project Lead |
  | Perham, Tom |Project Sponsor |
  | Roman, Daniel |Project Sponsor |
  | Roth, Daniel |Project Sponsor |

## Exercise 5: Develop below report
1. Think and create relations and get below output.

![image](https://user-images.githubusercontent.com/20516321/150071049-e7050e74-2c3e-4425-8fe4-60db6d951d69.png)


## Reference

https://docs.microsoft.com/en-us/power-bi/desktop-create-and-manage-relationships

https://docs.microsoft.com/en-us/power-bi/guidance/relationships-bidirectional-filtering

https://docs.microsoft.com/en-us/archive/blogs/cansql/relationships-in-power-bi-fixing-one-of-the-columns-must-have-unique-values-error-message

## Questions
----
1. What is composite models ?
  
    A model that combines data from more than one DirectQuery source or that combines DirectQuery with import data is called a composite model

    For more information refer [doc](https://docs.microsoft.com/en-us/power-bi/transform-model/desktop-composite-models#:~:text=A%20model%20that%20combines%20data,tables%20come%20from%20different%20sources.)

2. How many carinality's available?
  - One to One
  - One to Many
  - Many to One
  - Many to Many
    - Old versions of Power BI not supported. 
3. Fact to Dim what type of cardinality possible?
  - Many to One
4. Without Relationship, between two tables,will we get right data?
  - Wrong Data
5. Power BI creats relationships automatically based on what?
  - Column Names
6. Can you create Joins manually if column names are different?
  - Yes
7. Explain Single Vs Bi-directional Filters?
  - https://docs.microsoft.com/en-us/power-bi/guidance/relationships-bidirectional-filtering
8. What are the disadvantage of Bi-directional Join?
  - Negatively impact on model query performance
  - User confusing experiences
9. When to go for Bi-Directional Join? or Advantages of Bi-directional?
  - Special model relationships
    - one to one cardinality tables
    - Many to Many Cardinality Tables
    - **Note:** 99.99% we will have many to one relation tables in any dataset
  - Slicer items "with data"
  - Dimension-to-dimension analysis
  
  
   



```python

```
