1. Load **EMP** table data into power bi file

![image](https://user-images.githubusercontent.com/20516321/133961130-b49cbc4d-e56a-4238-b204-d7da2e29ec4f.png)

2. In **Report** View > Click on **Modeling** menu > Click on **New Parameter** > fill as shown below > Click on **ok**

![image](https://user-images.githubusercontent.com/20516321/133961334-37d3c4e5-489a-4fee-a6f8-e931b188e249.png)

3. Select **type of slicer** as **Dropdown** > Set **Single Select** option **ON**
4. Create a new Mesure with the name of **TotalSal**

![image](https://user-images.githubusercontent.com/20516321/133963158-8eedb205-dc36-43bc-b025-ed1967d66512.png)

5. Create one more new measure with the name of **Top N Sals**

`Top N Sals = 
VAR SelectedTop=SELECTEDVALUE('TopN'[TopN])
RETURN
SWITCH(TRUE(),SelectedTop=0 ,[TotalSal],RANKX(ALLSELECTED(EMP[ENAME]),[TotalSal])<=SelectedTop,[TotalSal])`

6. Create a table as shown below and test it.
![image](https://user-images.githubusercontent.com/20516321/133963649-6ca2d271-830d-44de-90f4-4e8f58b28367.png)

