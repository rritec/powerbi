
# Filter data with Power BI
1. In PowerBI filters are mainly **6** types
    - Slicer
    - Filter Pane Filters
        - Vizulations Level Filter
        - Page Level Filter
        - All Pages Level Filter or Report Level Filter
    - Drill Through Filter
    - RLS(Row Level Security)

3. Data is the core of Power BI. As you explore reports, each visual draws its underlying data from sources that often contain far more data than you need. 
4. Power BI offers several ways to filter reports. Knowing how to filter data is the key to finding the right information
![](https://docs.microsoft.com/en-us/learn/modules/analyze-data-power-bi/media/2-1/power-bi-filter-intro.gif)

## Slicers
1. A simple type of filtering that you can use directly on the report page is called a slicer.
1. There are several different types of slicers: **numeric**, **categorical**, and **date**. 
1. Slicers make it easy to filter all the visuals on the page at once.

    ![](https://docs.microsoft.com/en-us/learn/modules/analyze-data-power-bi/media/2-1/power-bi-slicers.gif)
1.If you want to select more than one field, hold the Ctrl key and click additional fields.    

## Explore the Filters pane
1. Another way to filter data is by opening and modifying filters in the Filters pane. The Filters pane contains filters that were added to the report by the report designer. As a consumer, you can interact with the filters and save your changes but can't add new filters.

The **four types** of filters are:

1. **Filter on all pages** or **Report Level Filter** > Applies to all pages in the report.
1. **Filter on this Page** or **Page Level Filter** – Applies to all the visuals on the current report page.
1. **Visual level Filter** – Applies to a single visual on a report page. You only see visual level filters if you've selected a visual on the report canvas.
1. **Drillthrough Filter** – Allows you to explore successively more detailed views within a single visual.
    ![](https://docs.microsoft.com/en-us/learn/modules/analyze-data-power-bi/media/2-1/power-bi-filter-types.png)

### Filter on all pages or Report Level Filter
1. Open **Labdata/Lab3/Lab 3 - Starting.pbix**
1. Click on **New page** and rename it as **USA Region Wise Sales**
1. In **Visulizations**> Click on **Table**
1. From **Fields** > select **Country**,**Region** and **Total Sales**
1. Our report will be looks like below image

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0072.png?raw=true)
1. Right click on **USA Region Wise Sales** > Click on **Duplicate Page**
1. Rename page as **USA Region Wise Units**
1. Delete column **Total Sales** and drag **Total Units**
1. Drag and drop **Country** column below **Filter on all Pages** > Select **USA** > observe reports data in both the pages
    
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0073.png?raw=true)

### Filter on this Page or Page Level Filter
1. In above report **USA Region Wise Sales** > drag and drop **year** column onto **Filters on this page** > show only sales **greater than or equal** to **2006** and **less than or equal** to **2010**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0074.png?raw=true)
    
1. Observe report data

### Filter on this Visual
1. In above report **USA Region Wise Sales** > select **table visulization** > provide region filter as shown in below image 

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0075.png?raw=true)
    
1. Observe report data


### Drill Through
1. Refer previous lesson


### Reference
[Refer and complete learning path](https://docs.microsoft.com/en-us/learn/modules/analyze-data-power-bi/1-filtering-data)

### Questions:
1. How many Filters available in Power BI?

    - Slicer
    - Filter Pane
        - Viz
        - page
        - all pages
    - Drill Through
    - Row-Level Security(RLS)
2. What is the defualt sorting in slicer?
    - Ascending order
1.  Slicer by default will affect other pages visulizations? do you have any work arounds?
    - No, we have work arounds [Refer](https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-visualization-slicers#sync-and-use-slicers-on-other-pages) 
1.  I have a slicer and two visulas ,slicers need to affect only one visual,is it possible?
    - Yes. [Refer](https://docs.microsoft.com/en-us/power-bi/visuals/power-bi-visualization-slicers#control-which-page-visuals-are-affected-by-slicers)
1. Can you create a slicer with two values "option1" and "option2"
    - Yes. create Custome table then create slicer using custom table [refer](https://docs.microsoft.com/en-us/power-bi/connect-data/desktop-enter-data-directly-into-desktop)
2. 
```python

```
