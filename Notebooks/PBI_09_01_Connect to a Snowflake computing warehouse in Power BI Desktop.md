
1. Create **Snowflake** data warehouse
    1. Sign up for free account
	- Click [here](https://signup.snowflake.com/?_ga=2.244222469.1468146556.1618626004-173092964.1618626004) and create id 
	- Provide all information like name and mailid  > click **Continue** > Choose your Snowflake edition as **Enterprise** > Choose your cloud provider as **Microsoft Azure** > Region as **West US2 (washington)** > click on **Get Started** > Open Mail > Verify mail to activate the account > create username and password
	![image](https://user-images.githubusercontent.com/20516321/115165273-bd052100-a0ca-11eb-89f9-a2443e23c786.png)

	- 
    
  
1. Open PBI Desktop
1. Connect snowflake
1. Server name copy from activation mail > xxxxxxxx.west-us-2.azure.snowflakecomputing.com
1. Warehouse > COMPUTE_WH > click on **ok**
2. provide username: xxxxxx  > pasword: xxxxxx > click on **connect**
3. Select Required Tables
4. Expand Snowflake_sample_data > expand TPCH_SF1 > select tables Customer, Nation, Region, Orders
5. Create joins accordingly.

![image](https://user-images.githubusercontent.com/20516321/230553459-aee3b83f-1f94-40fa-b8b6-baf135bbdde4.png)

6. Develop the report using columns region name ,nation name and total price.

![image](https://user-images.githubusercontent.com/20516321/230553939-dfc03b98-aebe-4b12-9a05-e5d3823b6c99.png)


7. 

    

**Optional:**

  1. Install snowsql CLI https://sfc-repo.snowflakecomputing.com/snowsql/bootstrap/1.2/index.html
  1. https://docs.snowflake.com/en/user-guide/getting-started-tutorial.html#snowflake-in-20-minutes
  
**Scripts:**

1. Know your account details, should be simillar to below

``` bash
account_name: ermwurj-md70724
account url : https://ermwurj-md70724.snowflakecomputing.com
username: mylarr9
password: RRitec***

```



1. open cmd
``` bash
snowsql -a uk00084.west-us-2.azure -u mylageethika
```
![image](https://user-images.githubusercontent.com/20516321/230555247-5e2d4fef-f799-4ccb-a010-a79de77bb053.png)

2. create a database
``` sql 

create or replace database sf_tuts;

```
3. know current database and schema
``` sql

select current_database(), current_schema();

```
4. create a table
``` sql 

CREATE OR replace TABLE emp_basic
                        (
                                                first_name string ,
                                                last_name string ,
                                                email string ,
                                                streetaddress string ,
                                                city string ,
                                                start_date date
                        );
 
```
  
  
5. Create compute warehouse
``` sql

create or replace warehouse sf_tuts_wh with
  warehouse_size='X-SMALL'
  auto_suspend = 180
  auto_resume = true
  initially_suspended=true;

```
  
6. Know cureent warehouse
``` sql

select current_warehouse();

```

7. put all files into staging location
``` bash

put file://c:\temp\employees0*.csv @sf_tuts.public.%emp_basic;

```

8. list the files in staging location

``` bash

list @sf_tuts.public.%emp_basic;

```
9. copy files from staging location to table

``` bash

copy into emp_basic
  from @%emp_basic
  file_format = (type = csv field_optionally_enclosed_by='"')
  pattern = '.*employees0[1-5].csv.gz'
  on_error = 'skip_file';

```
10. Observe all data

``` sql

select * from emp_basic;

```
11. insert few rows 

``` sql

INSERT INTO emp_basic
VALUES      ('Clementine',
             'Adamou',
             'cadamou@sf_tuts.com',
             '10510 Sachs Road',
             'Klenak',
             '2017-9-22'),
            ('Marlowe',
             'De Anesy',
             'madamouc@sf_tuts.co.uk',
             '36768 Northfield Plaza',
             'Fangshan',
             '2017-1-26'); 

```
12. Query data

``` sql

select email from emp_basic where email like '%.uk';

```

``` sql


select first_name, last_name, dateadd('day',90,start_date) from emp_basic where start_date <= '2017-01-01';

```

13. clean database and compute warehouse to save the credits (optional)

``` sql

drop database if exists sf_tuts;

```
``` sql

drop warehouse if exists sf_tuts_wh;

```
``` bash 

!exit

```

