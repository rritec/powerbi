# M-Language
--
1. Power Query Formula Language (informally known as "M")
2. **M** stands for **mash-up**
3. 
## Reference doc 
---
https://docs.microsoft.com/en-us/powerquery-m/quick-tour-of-the-power-query-m-formula-language

### Exercise 1: Write Simple M-languge Query
--
1. Open **Power Query Editor** > In Queries Pane > Right Click > New Query > Blank Query > Click on Advanced Editor > Then copy paste below code

        let
            x = 1 +1,
            y= 2+2,
            z = x+y+3
        in
            z
1. Click on done
2. Click on apply and close
3. develop report and observe output
### Exercise 2: Write Simple M-languge Query with spaces in variable name.
--
1. Replace above code with below code and observe result

       let
            x = 1,
            y = x * 10,
            #"variable name with spaces"=y+10
        in
            #"variable name with spaces"
            
 ### Exercise 3: Call functions in M-language
--
1. Replace above code with below code and observe result

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
### Exercise 4: Real world example
--
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

```M
= let 
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
in Sales2007[Total] + Sales2008[Total]

```
       
