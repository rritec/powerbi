
# Known Issues

## MySQL Public Key Retrieval is not allowed
1. Go to **DBeaver:**
1. Right click your connection, choose **Edit Connection**

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0028.png?raw=true)

1. On the **Connection settings** screen (main screen) click on **Edit Driver Settings**
1. Click on **Connection propertie**
1. Right click the **user properties** area and choose **Add new property**
1. Add two properties: **useSSL** and **allowPublicKeyRetrieval**
1. Set their values to  **false** and **true** by double clicking under the **value** column
   
   ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0029.png?raw=true)
    
1. Save and re-test the connection. Hopefully it should work!

    ![](https://github.com/rritec/powerbi/blob/master/images/PBI_0029.png?raw=true)


```python

```
