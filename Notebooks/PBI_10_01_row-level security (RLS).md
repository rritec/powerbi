
# Security
In any BI application 3 Tiers of Security required. Those are
1. Authentication
  - Application username and password is called as Authentication.
2. Autherization
  - Object Level (Workspace, App,Dashboard,Report,Dataset)
    - https://docs.microsoft.com/en-us/power-bi/collaborate-share/service-new-workspaces
    - https://docs.microsoft.com/en-us/power-bi/collaborate-share/service-roles-new-workspaces
  - Row Level Security(RLS) or Data Security 
# Row Level Security (RLS)

## Reference Documents

https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-rls



## Develop Data Security in Dynamic Way

1. Copy below data into Excel

| Item      | Price | Account Manager     |
| ---        |    ----   |          --- |
| Item 1      | 10       | studentpbi@mylaramreddy.onmicrosoft.com   |
| Item 2   | 20        | studentpbi@mylaramreddy.onmicrosoft.com      |
| Item 3   | 30        | vmyla1@mylaramreddy.onmicrosoft.com      |
| Item 4   | 40        | vmyla1@mylaramreddy.onmicrosoft.com      |

2. Save the excel as rritec_rls_source
3. Import the excel and develop a table report with three columns
![image](https://user-images.githubusercontent.com/20516321/114550670-15c65b00-9c80-11eb-8129-9e0bef38f3a4.png)

4. Click on the model > Click on the Manage Roles > Create a role as shown below
![image](https://user-images.githubusercontent.com/20516321/114550922-5d4ce700-9c80-11eb-91eb-afe79589603c.png)

5. Save this report as rls_report
6. Publish to workspace.
7. In the workspace make sure **info@datahexa.com** as **Viewer**
8. Go to Dataset > Security > Select **role** and map info@datahexa.com > Add > Save 
9. Open **Private window** in the brwoser > open app.powerbi.com > login using info@datahexa.com and password shared by your instructor.
10. Open the report and notice that only two records are visible
![image](https://user-images.githubusercontent.com/20516321/114551387-f24fe000-9c80-11eb-8dcd-0bfd582b64a4.png)



## Questions
1. RLS will applies to Workspace members assigned Admin, Member, or Contributor ?
  - No . Only applies on Viewers
2. 
```python

```
