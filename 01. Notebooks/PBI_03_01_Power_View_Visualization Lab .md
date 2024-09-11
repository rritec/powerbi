
# Power BI Desktop Visualization 

## Exercise 1- Cross-Tabular Report
- **Scenario:** You want to show VanArsdel's sales (revenue) and units for each month and year in a single report. You choose to show this using two Matrix visualizations.

1. Open file **Labdata/Lab3/Lab 3 - Starting.pbix** file.
1. In the navigation pane on the left, click **Report**.
1. In the **FIELDS** list, on the right, click the **Sales** table.
1. Drag the **Total Sales** field from the **Sales** table to the report to create a chart.
1. In the FIELDS list, on the right, click the **Date** table.
1. Drag the **MonthName** and **Year** fields from the **Date** table to the chart.
1. In the **VISUALIZATIONS** list, click **Matrix**.
1. In the **VISUALIZATIONS** list, in **Rows**, select **MonthName**, in **Columns**, select **Year**, and in **Values**, select **Total Sales**.
1. Click in the empty space of report
1. Repeat Step 3 to 8 to add another chart, but this time, display the **Total Units** field in place of **Total Sales**.
1. From the **Home** ribbon, click **Text** box.
1. In the text box, type **VanArsdel Sales and Units** and resize and move the text box so that it appears as the title of the report.
1. At the bottom of the screen, right-click **Page 1**, and click **Rename** Page.
1. Type **Sales and Units** and press **Enter**.
1. You should have something similar to the below Image:
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0023.png?raw=true)
1. Click **Save**, to save the Power BI file.    
### Think few mins, how to get below vizulization.

![image](https://user-images.githubusercontent.com/20516321/125020165-f9c33180-e095-11eb-9276-bf6689b976e9.png)

- Drag **Matrix** to work area
- Drag Year, Manufacturer, Region to **Rows**
- Drag **TotalSales** to **Values**
- Filter on **year** for **2001** and **2002**
- Filter on **region** for **Central** and **East**
- Filter on **Manufacturer** for **Abbas** and **Aliqui**
- Click **twice** on **Expand all down one level in the hierarchy**
- If you need **SubTotals** in the bottom set it in **format** tab

## Exercise 2- Part-to-Whole Report
**Scenario:** analyzing sales data by product category, segment and manufacturer.

1. Create a new report page by clicking **New Page (+)** at the bottom of the report view.
1. Drag the **Total Sales** field from the **Sales** table to the report and create a chart.
1. Drag the **Category** and **Segment** fields from the **Products** table to the chart.
1. In the **VISUALIZATIONS** list, click **100% Stacked Bar Chart** .
1. In the **VISUALIZATIONS** list, in **Axis**, select **Category**, in **Legend**, select **Segment**, and in **Value**, select **Total Sales**.
1. In the **VISUALIZATIONS** list, click the **Format** button.
1. Set **Data labels** to **On**.
1. Set **Value decimal places** to **0**.
1. Click on the empty space of report
1. Drag the **Total Sales** field from the **Sales** table to the report and create another chart.
1. Drag the **Manufacturer** field from the **Manufacturers** table to the chart.
1. Modify the chart to use the **Treemap visualization**.
1. Click on the empty space of report
1. Drag the **MonthName** field from the **Date** table to the report and create another chart.
1. Modify the chart to use the **Slicer visualization**.
1. Click on the empty space of report
1. Drag the **Year** field from the **Date** table to the report and create a chart.
1. Modify the chart to use the **Slicer visualization**.
1. Rename the report sheet to **Sales Breakdown**.
1. Click **Save**, to save the Power BI file.
1. You should have something similar to the below image:

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0024.png?raw=true)

## Edit Interactions:
Scenario: Slicer should not impact few vizulations.
- By Default Slicer changing all the visulizations inside the current page
- In above report click on year slicer > go to **Format** > click on **edit Interactions**  > select required vizulization **None** button.
- Now change any slicer options and observe the vizulation is not impacting.

## Sync Slicers
- In above report,copy any vizulaion and paste into other page .
- Go to view menu > click on **sync Slicers**
- select **year** slicer > select sync check boxes of current page and the pages need to impact.
- Change slicer options and observe that visulization changes.

## Exercise 3- Relationship Report

- **Scenario:** You would like to know more about the relationship between total units and total sales by category and segment. You choose to analyze this using scatter chart.

1. Create a new report page by clicking **New Page** at the bottom of the report view.
1. In **VISUALIZATIONS**, click **Scatter Chart**.
1. Drag the **Total Sales**, **Total Units**, and **YTD Sales** fields from the **Sales** table to the chart.
1. Drag the **Category** and **Segment** fields from the **Products** table to the chart.
1. Drag the **Year** field from the **Date** table to the chart.
1. Rename the report sheet to **Sales Relationship**.
1. Ensure that the following fields are set in the visualization Details:
    - Details: Category
    - Legend: Segment
    - X Axis: Total Sales
    - Y Axis: Total Units
    - Size: YTD Sales
    - Play Axis: Year
1. Click **Save**, to save the Power BI file.
1. You should have something similar to the below image:
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0025.png?raw=true)

## Exercise 4- Trend Report
**Scenario:** Show a chart to compare Total Sales and Total Units throughout the years. And then let's show two more charts showing the Total Sales and Total Units variances throughout the years.

1. Create a new report page by clicking the **New Page** icon at the bottom of the report view.
1. Drag the **Year** field from the **Date** table to the report and create the first chart.
1. Drag the **Total Sales** and **Total Units** fields from the **Sales** table to the Year chart.
1. Modify the chart to use the **Line and Stacked Column Chart** visualization.
1. Ensure that the **Year** is shown as the **Shared Axis**, **Total Sales** is shown as the **Column values**, and **Total Units** is shown as the **Line values** of the visualization Details.
----
1. Create a second chart based on the **Waterfall** Chart visualization.
1. Drag the **Sales Var** field from the **Sales** table to the Sales Var chart.
1. Drag the **Year** field from the **Date** table to the Sales Var chart.
---
1. Create a third chart, also based on the Waterfall Chart visualization.
1. Drag the **Total Units Var** field from the **Sales** table to the Total Units Var chart.
1. Drag the **Year** field from the **Date** table to the Total Units Var chart.
1. Click the Elipse button on both the Sales Var and Total Units Var charts and sort by **Year** ascending.
1. Add a **Text Box** to the report and enter **Yearly Trend** as the text.
1. Rename the report sheet to **Yearly Trend**.
1. Click **Save**, to save the Power BI file.
1. You should have something similar to the below image:

![](https://github.com/rritec/powerbi/blob/master/images/PBI_0026.png?raw=true)

## Exercise 5- Rank Report
**Scenario:** You now want to analyze individual products sales (revenue) and volume (units). You decide to show these using two bar charts.

1. Create a new report page by clicking the **New Page** icon at the bottom of the report view.
1. Drag the **Total Sales** field from the **Sales** table to the report and create a chart.
1. Drag the **Product** field from the **Products** table to the chart.
1. Modify the chart to use the **Stacked Bar Chart** visualization.
1. Ensure that the chart is sorted by **Total Sales**.
----
1. Click on empty space of report
1. Drag the **Total Units** field from the **Sales** table to the report and create a new chart.
1. Drag the **Product** field from the **Products** table to the chart.
1. Modify the chart to use the **Stacked Bar Chart** visualization.
1. Ensure that the chart is sorted by **Total Units**.
-----
1. Click on empty space of report
1. Drag the **Year** field from the **Date** table to the report and create a new chart.
1. Modify the chart to use the **Slicer visualization**.
1. Modify the slicer type by clicking the **dropdown** arrow in the Year chart and selecting the **List** option.
1. Add a **Text Box** to the report and enter **Top Products** as the text.
1. Rename the report sheet to **Top Products**.
1. Click **Save**, to save the Power BI file.
1. You should have something similar to the below image:
![](https://github.com/rritec/powerbi/blob/master/images/PBI_0027.png?raw=true)

## Reference

https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-report-visualizations

## Exercise 1:

![image](https://user-images.githubusercontent.com/20516321/115183931-64e61300-a0fa-11eb-9740-bc7eebf4f56a.png)

## Exercise 2:

https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-visualization-radial-gauge-charts

```python

```
