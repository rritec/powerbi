
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

```python

```
