
# Row Level Security (RLS)

## Reference Documents

https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-rls

## Develop Data Security in Static Way

1. Copy below data into Excel

| Item      | Price | Account Manager     |
| ---        |    ----   |          --- |
| Item 1      | 10       | ramreddy1@datahexa.com   |
| Item 2   | 20        | ramreddy1@datahexa.com      |
| Item 3   | 30        | info@datahexa.com      |
| Item 4   | 40        | info@datahexa.com      |

2. Save the excel as rritec_rls_source
3. Import the excel and develop a table report with three columns
![image](https://user-images.githubusercontent.com/20516321/114550670-15c65b00-9c80-11eb-8129-9e0bef38f3a4.png)

4. Click on the model > Click on the Manage Roles > Create **Four** role as shown below
![image](https://user-images.githubusercontent.com/20516321/114554400-4f996080-9c84-11eb-9830-322389658f0b.png)


5. Save this report as rls_report_static
6. Publish to workspace.
7. In the workspace make sure **info@datahexa.com** as **Viewer**
8. Go to Dataset > Security > Select item 3 and map info@datahexa.com > add > save > Select item 3 and map info@datahexa.com > add > save
9. Open **Private window** in the brwoser > open app.powerbi.com > login using info@datahexa.com and password shared by your instructor.
10. Open the report and notice that only two records are visible
![image](https://user-images.githubusercontent.com/20516321/114551387-f24fe000-9c80-11eb-8dcd-0bfd582b64a4.png)

## Develop Data Security in Dynamic Way

1. Copy below data into Excel

| Item      | Price | Account Manager     |
| ---        |    ----   |          --- |
| Item 1      | 10       | ramreddy1@datahexa.com   |
| Item 2   | 20        | ramreddy1@datahexa.com      |
| Item 3   | 30        | info@datahexa.com      |
| Item 4   | 40        | info@datahexa.com      |

2. Save the excel as rritec_rls_source
3. Import the excel and develop a table report with three columns
![image](https://user-images.githubusercontent.com/20516321/114550670-15c65b00-9c80-11eb-8129-9e0bef38f3a4.png)

4. Click on the model > Click on the Manage Roles > Create a role as shown below
![image](https://user-images.githubusercontent.com/20516321/114550922-5d4ce700-9c80-11eb-91eb-afe79589603c.png)

5. Save this report as rls_report
6. Publish to workspace.
7. In the workspace make sure **info@datahexa.com** as **Viewer**
8. Open **Private window** in the brwoser > open app.powerbi.com > login using info@datahexa.com and password shared by your instructor.
9. Open the report and notice that only two records are visible
![image](https://user-images.githubusercontent.com/20516321/114551387-f24fe000-9c80-11eb-8dcd-0bfd582b64a4.png)



## Questions
1. RLS will applies to Workspace members assigned Admin, Member, or Contributor ?
  - No . Only applies on Viewers
2. 
```python

```
