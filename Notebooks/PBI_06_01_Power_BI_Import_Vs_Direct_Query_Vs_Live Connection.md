
https://docs.microsoft.com/en-us/power-bi/power-bi-data-sources

Example:

Excel has no direct Query

Sql Server has Direct query

![image](https://user-images.githubusercontent.com/20516321/113528602-a779fc80-95de-11eb-938a-3808cc990206.png)


![image](https://user-images.githubusercontent.com/20516321/113528740-1d7e6380-95df-11eb-9d46-946971a3287a.png)


https://radacad.com/directquery-live-connection-or-import-data-tough-decision
https://docs.microsoft.com/en-us/power-bi/connect-data/desktop-directquery-about

	Import(90%)	Direct Query/Live Connection(10%)	Comments
Memory(Hard Disk Space)	(metadata + Data)2044KB	(Metadata)32KB	"1. Publish Limitation of PBIX file is 1GB
2. PBIS Storage follows Column-store in-memory technology"
Performance	High Speed	Low Speed	
Features	All Dax Functions using possible	Few Dax Functions using possible	
![image](https://user-images.githubusercontent.com/20516321/183326168-df918024-1b3e-42c1-aa85-b0a2042cf906.png)


## Questions
---
1. How many types of connection available in Power BI
  - Import
  - Direct Query
  - Live Connection
  - Stream
2. What is the size limit of dataset in power BI Service Pro ?
  - 1GB
3. For Each Power BI Service, what is the total size limit of datasets?
  - 10 GB
4. Data inside PBIX file stores in what format?
  - Columnar Store
  - Compresed format(Due to this Size will be reduced to approximately below 10% actual size)
  
5. Import Data Connection Pros and Cons
  - Pros
    - Power BI Fully Functional
      - we can use time intilligency functions
      - Query combineing
      - ...etc
    - Performance is very good as data already available inside poer bi service
    - it is possible with all data sources(file/Databases/web/...etc)
  - Cons
    - Size limitations
    - Shedule data sets by following ETL data refresh window
  
6. Direct Query/Live Connection Connection Pros and Cons
  - Pros
    - No need of schudling dataset always we will get latest data from database
    - No Hard disk space or power Bi service space consumed
  - Cons
    - Can not support all data sources
    - Performance is not good as it as to run query in the runtime and fetch results from database
    - Power BI all fetures are not supported
7. Always give first priority to Import connection
8. Live connection available only for SSAS Tabular Models and SSAS Multidimensional Cubes
9. Can you swtich Import Connection of table to Direct Query?
  - No
10. Can you swtich Direct Query Connection of table to Import?
  - Yes
 11. What is Dual Storage, when we will use it.
  - https://docs.microsoft.com/en-in/power-bi/transform-model/desktop-storage-mode


```python

```
