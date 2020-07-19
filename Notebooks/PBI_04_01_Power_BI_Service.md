
# Power BI Service

## Exercise 1- Upload PBI Report and Pin Visualizations

1. Open the **Labdata/Lab4/Lab 4 Starting.pbix** file.
1. On the **Home ribbon**, click **Publish**.
1. In Select a destination, select **My workspace**, and click **Select**.
1. If prompted, sign in using the account you used to sign up for the Power BI service.
1. [Signup link](https://signup.microsoft.com/signup?sku=a403ebcc-fae0-4ca2-8c8c-7a907fd6c235&email=&ru=https%3A%2F%2Fapp.powerbi.com%3Fpbi_source%3Dweb_nolicense_redirect%26redirectedFromSignup%3D1%26noSignUpCheck%3D1)
1. Once the report is published, click Got it.
1. Start an Internet browser, go to https://app.powerbi.com/, and click Sign in.
1. Sign in using your account.
1. Go to the **Lab 4 Starting Report** and explore your published report. It looks similar to the one in Power BI Desktop file. Now you can start creating a dashboard by pinning some visualizations.
1. Go to the **Sales Report** tab and pin the chart showing **Total Sales by Category and Segment** (100% Stacked Bar Chart). Select to create a New dashboard and name it **VanArsdel Sales**.
1. Pin the **treemap chart**, **the scatter chart**, and the **map** visualization from the Sales Report tab to the **VanArsdel Sales** dashboard.
1. Go to the **Yearly Trend** tab and pin the **waterfall chart** that shows the **Sales Var by Year** to the VanArsdel Sales dashboard.
1. Go to the VanArsdel Sales dashboard and review what you have created.
1. Resize and arrange the tiles as necessary.
1. On the top-right, click Web view and click Phone view.
1. Review the phone view.
1. Resize and arrange the tiles as necessary.
1. You should have something similar to the below image:

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0048.png?raw=true)

## Exercise 2- Share Dashboard and Update Report

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
---
1. **Home Work**
1. Once you've uploaded your Power BI Desktop file to Power BI service, you can still make changes to it, and re-upload the file so that your changes is reflected in Power BI service.
1. Open the **Lab 4 Starting.pbix** file.
1. Modify the **Total Sales by Category and Segment chart** (the one displayed using **100% stacked bar chart** visualization) on the Sales Report tab to use **Stacked Bar chart** visualization instead.
1. Again **publish** the file to **Power BI service** and replace the existing dataset with this one.
1. Go to Power BI service and review the **Lab 4 - Starting Report** and examine whether the change you made is reflected.

## Exercise 3- Schedule Data Refresh

1. So far, the report you uploaded is rather **static**. That means, if the data in the Access database changes, the report and dashboard are not updated. You can install **Power BI Personal Gateway** and schedule data refresh for on-premises data sources, such as the Access database, to keep your report and dashboard on Power BI service **up-to-date**.

1. NOTE: Power BI Pro is required to setup scheduled refresh for on-premises data. If you do not have Power BI Pro subscription you can enroll for a free 60 day trial.

1. On the Power BI website, click My Workspace, click Datasets, click Lab 4 – Starting, and click the Schedule refresh icon.
1. Power BI Pro is required to setup scheduled refresh for on-premises data. If you do not have Power BI Pro subscription you can enrol for a 60 day trial.
1. Ensure that you are in the Datasets tab and that the Lab 4 - Starting dataset is selected.
1. Click Gateway connection and click Install now to download the Power BI Personal Gateway.
1. When the download is complete, click the On-premises data gateway to begin installation.
1. Click Next, accept the license terms, and click Install.
1. Sign in using your Power BI account and click Close.
1. In New on-premises data gateway name, type Van Arsdel Sales.
1. In Recovery key and Confirm recovery key, type Pa$$w0rd, and click Configure.
1. Click Close.
1. Expand Data source credentials and, for Country Population by Year.xlsx, click Edit credentials.
1. For Privacy level setting for this data source, select Organizational, and click Sign in.
1. Edit credentials for the Data sources that needs updating.
1. Now you can schedule your data source refresh.
1. NOTE: If you are using the starter file provided in the beginning of Lab 4, in order to be able to successfully refresh the data, please ensure that you have the files from previous labs under the "C:\DAT207x" folder. This is because the files were developed with this referenced. You might use arbitrary folders in your own scenario or if you are using your own file throughout the labs.

## Exercise 4: Add Youtube Video using Tile
1. In above report click on **...** > Click on **+ Add tile**
1. Under Media, Clic on **Web Content**  > Select **Next** 
1. Under **Embed Code** > paste below code 
```html
<object width="425" height="355"><param name="movie" value="https://www.youtube.com/v/4_afKAWj2Ek&hl=en"></param><param name="wmode" value="transparent"></param><embed src="https://www.youtube.com/v/4_afKAWj2Ek&hl=en" type="application/x-shockwave-flash" wmode="transparent" width="425" height="355"></embed></object>

        
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0125.png?raw=true)

1. Click om **Apply** and observe Tile in the dashboard

## Exercise 5: Add Image Tile

1. In above report click on **...** > Click on **+ Add tile**
1. Under Media, Clic on **Image**  > Select **Next** 
1. Under **Content** > paste below URL

    https://github.com/rritec/datahexa/blob/master/images/Mentor_dl.jpg?raw=true

1. Click om **Apply** and observe Tile in the dashboard    

## Exercise 6: Add youtube Video

1. In above report click on **...** > Click on **+ Add tile**
1. Under Media, Clic on **Video**  > Select **Next** 
1. Under **Content** > paste below URL

    https://youtu.be/K40PGTYM2i0

1. Click om **Apply** and observe Tile in the dashboard    

## Exercise 7: Explan Dasboard Themes

1. In above report click on **...** > Click on **Sashboard Theme** > explore it
  

## Exercise 8: Apps

1. Explore it https://docs.microsoft.com/en-us/power-bi/service-organizational-content-pack-create-and-publish
  


```python

```
