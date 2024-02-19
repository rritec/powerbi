
# Hierarchy

- Can you use **drill down/drill up** without **Hierarchy** ?
    - <input type="radio" disabled> Yes
    - <input type="radio" disabled checked> No
- Without Creating Hierarchy, can you drill down from **Category** to **segment** to **product**?   
    - <input type="radio"> Yes
    - <input type="radio" checked> No

## Exercise 1: Develop a report **Total Sales by Category**
- from fileds select total Sales and Category columns 
- select Stacked Column Chart
- Click on any bar to  move from category to segment. Are you able to move ??? no right??? so let us learn how to create hierarchy

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0049.png?raw=true)

## Create Product Hierarchy

- In **Fields** Pane
- Expand **Product** table
- Select **Segment** and drag and drop on to **Category**
- Observe one hierarchy created with the name ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0050.png?raw=true)
- Rename **Category Hierarchy** as **Product Hierarchy**
- Select **product** Column and drop onto **Product Hierarchy**
- Finally your hierarchy will be looks like this

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0053.png?raw=true)



## Understanfd below terms and functionalties
    1. Drill Down
    2. Drill Up
    3. Show Next Level
    4. Expand Next Level
    
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0054.png?raw=true)

### Drill Down

    - Navigating from high level data to low level data (Example : Year > Half Year > Quarter > Month > Day)

1. In **Visulizations** > Click on **Stacked Column Chart**
1. From **Fields** pane > Click on **Total Sales** and **Product Hierarchy** 
1. Your report should look as shown below

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0055.png?raw=true)
    
1. **Click to turn on drill down** as shown below

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0056.png?raw=true)
1. Click on **Urban** bar and observe urban related **Segment** sales

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0057.png?raw=true)



### Drill Up

    - Navigating from low level data to high level data (Example : Day > Month > Quarter > Half Year > Year)
1. Click on **Drill Up** to see again **Category** Level Data

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0058.png?raw=true)

### Show Next Level
- Rolls data to next level irrespective of category

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0061.png?raw=true)

### Expand Next Level
- Shows category-Segment Data
    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0062.png?raw=true)


```python

```
