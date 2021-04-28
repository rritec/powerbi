# M-Language
--

## Reference doc 
---
https://docs.microsoft.com/en-us/powerquery-m/quick-tour-of-the-power-query-m-formula-language

https://radacad.com/basics-of-m-power-query-formula-language

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
