
1. Create **Snowflake** data warehouse
    1. Sign up for free account
	- Click [here](https://signup.snowflake.com/?_ga=2.244222469.1468146556.1618626004-173092964.1618626004) and create id 
	- Provide all information like name and mailid  > click **Continue** > Choose your Snowflake edition as **Enterprise** > Choose your cloud provider as **Microsoft Azure** > Region as **West US2 (washington)** > click on **Get Started** > Open Mail > Verify mail to activate the account > create username and password
	![image](https://user-images.githubusercontent.com/20516321/115165273-bd052100-a0ca-11eb-89f9-a2443e23c786.png)

	- 
    
  
1. Open PBI Desktop
1. Connect snowflake
		1. Server > xxxxxxxx.west-us-2.azure.snowflakecomputing.com
		2. Warehouse > COMPUTE_WH > click on **ok**
		3. provide username: xxxxxx  > pasword: xxxxxx > click on **connect**
		
1. Select Required Table

	1. Expand Snowflake_sample_data > expand TPCH_SF1 > select tables Customer,Nation,Region,Orders
	1. Create joins accordingly.

    
1. Develop the report using columns region name ,nation name and total price.

    

**Optional:**

  1. Install snowsql CLI https://sfc-repo.snowflakecomputing.com/snowsql/bootstrap/1.2/index.html
  1. https://docs.snowflake.com/en/user-guide/getting-started-tutorial.html#snowflake-in-20-minutes
**Scripts**
```
account_name: bk73213.west-us-2.azure
account url : https://BK73213.west-us-2.azure.snowflakecomputing.com
sername: mylavenkata1
password: Apr@2021



snowsql -a bk73213.west-us-2.azure -u mylavenkata1
create or replace database sf_tuts;
select current_database(), current_schema();
create or replace table emp_basic (
  first_name string ,
  last_name string ,
  email string ,
  streetaddress string ,
  city string ,
  start_date date
  );
  
  
create or replace warehouse sf_tuts_wh with
  warehouse_size='X-SMALL'
  auto_suspend = 180
  auto_resume = true
  initially_suspended=true;
  
select current_warehouse();

put file://c:\temp\employees0*.csv @sf_tuts.public.%emp_basic;

list @sf_tuts.public.%emp_basic;
copy into emp_basic
  from @%emp_basic
  file_format = (type = csv field_optionally_enclosed_by='"')
  pattern = '.*employees0[1-5].csv.gz'
  on_error = 'skip_file';
select * from emp_basic;
insert into emp_basic values
  ('Clementine','Adamou','cadamou@sf_tuts.com','10510 Sachs Road','Klenak','2017-9-22') ,
  ('Marlowe','De Anesy','madamouc@sf_tuts.co.uk','36768 Northfield Plaza','Fangshan','2017-1-26');
select email from emp_basic where email like '%.uk';
select first_name, last_name, dateadd('day',90,start_date) from emp_basic where start_date <= '2017-01-01';

drop database if exists sf_tuts;

drop warehouse if exists sf_tuts_wh;

```

