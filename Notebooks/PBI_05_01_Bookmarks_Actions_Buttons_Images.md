

# Reading Activity:
https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-bookmarks

https://docs.microsoft.com/en-us/power-bi/create-reports/desktop-buttons


## Use Case 1: Clear All Slicers in Power BI
----
1. Create a **text box** and name it as Dname:
1. Create a **Slicer** with Dname Column
1. Create a **text box** and name it as Job:
1. Create a **Slicer** with Job Column
1. Develop a pie chart location by salary 
1. Develop a pie chart Ename by salary 
1. Kepp two slicers with all option
1. Go to view menu create a book mark and rename it has **Clear All**
1. Create a **Blank** Button > Select it change **Button Text** as **Clear All** > Select **action** as **Clear All** book mark
1. Change slicers as you wish  and observe data
1. press ctrl and click on button it will reset all slicers to **all**

![image](https://user-images.githubusercontent.com/20516321/209264366-34062b18-eeb1-4b6f-a76c-47e16aab8464.png)

## Use Case 2: Toggle between Pie and Bar Chart
----
1. Open Power BI Desktop
2. Import DimCustomer.csv and FactInternetSale.csv
3. Develop a pie chart and column chart one overap another
4. Change titles of visulizations as Pie and Bar respectively
5. Open Selection pane and Bookmarks pane
6. Hide Column chart and create bookmark as Pie
7. Hide Pie chart and create bookmark as Column
8. From google download two images Pie and bar chart
9. Go to insert menu and click on images and browse above pie and place in the work area as small as possible
10. Go to insert menu and click on images and browse above bar and place in the work area as small as possible
11. Select Pie image > enable Actions > select bookmarks as pie
12. Select Bar image > enable Actions > select bookmarks as Bar
13. Test it

![image](https://user-images.githubusercontent.com/20516321/113813419-7b50ae00-978d-11eb-9718-acd2f1cc6c79.png)

## Use Case 3: Navigate to required page of PBIX file Dynamically
----

- Create custom table by using Enter Table option
    - In **Power BI Desktop** > Click on **Enter Data** > Provide **Table Name**, **Column Name** and Values must be equal to your PBIX page names 
    - For Example
        ![image](https://user-images.githubusercontent.com/20516321/116339897-e117df00-a7fb-11eb-95eb-517087b67597.png)
- Develop a slicer using above column and make it as single selection
- Introduce one Image and allign beside slicer as shown below image
- select Image > Go to format > action > Type: **Page Navigation** > Destination: Click on **Fx** > Format By: **Field Value** > Based on Field: **Select column what you created** > Click on **ok**


![image](https://user-images.githubusercontent.com/20516321/113814794-d1beec00-978f-11eb-9e36-7511da5f7002.png)


1. **Reference**
    https://radacad.com/clear-all-slicers-in-power-bi-a-bookmark-story
    
    https://radacad.com/bookmarks-and-buttons-making-power-bi-charts-even-more-interactive
    
