
# Power BI Service

## Create a new workspace

1. Signup for new user id and password with **work mail id** [Signup link](https://signup.microsoft.com/signup?sku=a403ebcc-fae0-4ca2-8c8c-7a907fd6c235&email=&ru=https%3A%2F%2Fapp.powerbi.com%3Fpbi_source%3Dweb_nolicense_redirect%26redirectedFromSignup%3D1%26noSignUpCheck%3D1) or **use what instructor provided to you**.
2. Open https://app.powerbi.com/
3. Signin with username and password given to you by your instructor
    ![image](https://user-images.githubusercontent.com/20516321/112792985-1658d200-9082-11eb-9f74-63b862b27d24.png)

4. In the left **Navigation Pane** > Click on **Workspaces** > Click on **Create a Workspace** > provide **workspace name** as **rritec-workspace** > click on **Save**

## Publish PBI Report

1. Open the **Labdata/Lab4/Lab 4 Starting.pbix** file.
1. On the **Home ribbon**, click **Publish**.
1. In Select a destination, select **rritec-workspace**, and click **Select**.
1. If prompted, sign in using the account you used to sign up for the Power BI service.
1. [Signup link](https://signup.microsoft.com/signup?sku=a403ebcc-fae0-4ca2-8c8c-7a907fd6c235&email=&ru=https%3A%2F%2Fapp.powerbi.com%3Fpbi_source%3Dweb_nolicense_redirect%26redirectedFromSignup%3D1%26noSignUpCheck%3D1)
1. Once the report is published, click Got it.
1. Open browser, go to https://app.powerbi.com/, and click Sign in.
1. Sign in using your account.
1. Go to the **Lab 4 Starting Report** and explore your published report. It looks similar to the one in Power BI Desktop file. Now you can start creating a dashboard by pinning some visualizations.
## Create Dashboard by Pining Visualizations
1. Go to the **Sales Report** tab and pin the chart showing **Total Sales by Category and Segment** (100% Stacked Bar Chart). Select to create a New dashboard and name it **VanArsdel Sales**.
1. Pin the **treemap chart**, **the scatter chart**, and the **map** visualization from the Sales Report tab to the **VanArsdel Sales** dashboard.
1. Go to the **Yearly Trend** tab and pin the **waterfall chart** that shows the **Sales Var by Year** to the VanArsdel Sales dashboard.
1. Go to the VanArsdel Sales dashboard and review what you have created.
1. Resize and arrange the tiles as necessary.
1. Go to **Edit** > Click on **Mobile Layout** > Observe how it looks in mobile > In the Right Side corner Click on **Web Layout** to see how it looks in web/laptops
1. Review the phone view.
1. Resize and arrange the tiles as necessary.
1. You should have something similar to the below image:

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0048.png?raw=true)
    
- **Note:** If the original visualization that's used to create the tile changes, the tile doesn't change. For example, if you pin a line chart from a report and then you change the line chart to a bar chart, the dashboard tile continues to show a line chart. The data refreshes, but the visualization type doesn't.

## Share Dashboard

1. Let's start sharing your newly created dashboard. For simplicity, let's share the dashboard to your own email address.

1. **NOTE:** Power BI Pro is required for sharing dashboards. If you do not have a Power BI Pro subscription, you can enroll for a free 60 day trial.

1. Click **My Workspace**, click Dashboards, and click **Van Arsdel Sales**.
1. In the **VanArsdel Sales** dashboard, click the **Share** button to share your dashboard.
1. Click **Try Pro** for free.
1. Click **Start Trial**, and click **Close**.
1. Click **My Workspace**, click **Dashboards**, and click **Van Arsdel Sales**.
1. In the **VanArsdel Sales dashboard**, click the **Share** button to share your dashboard.
1. In Grant access to, enter your email address used for Power BI service and click Share.
1. Check your inbox to see an invite to view this dashboard.

## Update Report and re-publish
----
1. Once you've published your Power BI Desktop file to Power BI service, you can still make changes to it, and re-publish the file so that your changes is reflected in Power BI service.
1. Open the **Lab 4 Starting.pbix** file.
1. Modify the **Total Sales by Category and Segment chart** (the one displayed using **100% stacked bar chart** visualization) on the Sales Report tab to use **Stacked Bar chart** visualization instead.
1. Again **publish** the file to **Power BI service** and replace the existing dataset with this one.
1. Go to Power BI service and review the **Lab 4 - Starting Report** and examine whether the change you made is reflected.

## Add entire page to dashboard as live page
1. Open report > click on **...** > Click on **Pin to a dashboard**
 
## Add Web Content Tile
----
4. Web Content Tile accepts any html tags/code
5. In above report click on **Edit** > Click on **+ Add tile**
6. Under Media, Clic on **Web Content**  > Select **Next** 
7. Under **Embed Code** > paste below code html

    ```
    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>
    ```

1. Click om **Apply** and observe Tile in the dashboard

## Add Image Tile
-----

1. In above report click on **Edit** > Click on **+ Add tile**
1. Under Media, Clic on **Image**  > Select **Next** 
1. Under **Content** > paste below URL

    https://github.com/rritec/datahexa/blob/master/images/Mentor_dl.jpg?raw=true

1. Click om **Apply** and observe Tile in the dashboard    

## Add youtube Video
----

1. In above report click on **Edit** > Click on **+ Add tile**
1. Under Media, Clic on **Video**  > Select **Next** 
1. Under **Content** > paste below URL

    https://youtu.be/DNovBg5VCHA?list=PLpF-Cn8-Vi9QLt3NsK-7RH0jUPGRLnu7o

1. Click om **Apply** and observe Tile in the dashboard    

## Explore Dasboard Themes
----

#### Exercise 1: Export and import custom theme.

1. Open **PowerBI Desktop** > Open Any **report** > Go to **View** menu > Click on **Themes** down arrow mark > Click on **Customize Current Theme**
2. Observe all **properties**
3. Change required **colors** or **fonts** ...etc
4. Click on **Apply**
5. Again Go to **View** menu > Click on **Themes** down arrow mark > **Save Current Theme** into local pc **Desktop**
6. Open any other report > Go to **View** menu > Click on **Themes** down arrow mark > Click **Browse for themes** > Select previously saved **json** file > Click on **open** > observe changes

#### Exercise 2: Change Themes from Power BI Service.

1. In above report click on **Edit** > Click on **Dashboard Theme** > explore it

    - For more info [click here](https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-report-themes)
  

## Questions
1. Without using **Power BI Desktop**, will you be able to upload **PBIX** file into **Power BI Service** ?
    - Yes. 
    - Go to required **workspace** > Click on **New** > Click on **Upload a File**
        ![image](https://user-images.githubusercontent.com/20516321/114537204-8e70eb80-9c6f-11eb-9c72-a4f0d0b68c5c.png)

2. 

  
