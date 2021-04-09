
# Data Refresh
---

1. What are the connection types?
  - Import
      - Today 10 rows available in the excel/sql server/oracle/teradata(on - Permise Datasets)
      - you imported to PBI file
      - Developed reports
      - published report to power Bi service
      - After one month  5 more records added to excel and 2 records of excel updated and 1 record of excel deleted.Now total number of records in excel is 14
      - However if i go and run report in **power Bi service** ,iam seeing old data (10 rows). How to fix it?
      - 
  - Direct Query
  - Live
  - Stream
2. Power BI Service(Azure Cloud) Communicates On -Permise Datasets using ?
  - Gateway
## What is an on-premises data gateway?
- The on-premises data gateway acts as a bridge to provide quick and secure data transfer between on-premises data (data that isn't in the cloud) and several Microsoft cloud services.
- These cloud services include Power BI, PowerApps, Power Automate, Azure Analysis Services, and Azure Logic Apps.
- By using a gateway, organizations can keep databases and other data sources on their on-premises networks, yet securely use that on-premises data in cloud services.

![image](https://user-images.githubusercontent.com/20516321/113988805-74996800-986d-11eb-888f-c7255a071f55.png)

## Types of gateways
- There are two different types of gateways, each for a different scenario:

  1. **On-premises data gateway** allows multiple users to connect to multiple on-premises data sources. You can use an on-premises data gateway with all supported services, with a single gateway installation. This gateway is well-suited to complex scenarios with multiple people accessing multiple data sources.

  2. **On-premises data gateway (personal mode)** allows one user to connect to sources, and can’t be shared with others. An on-premises data gateway (personal mode) can be used only with Power BI. This gateway is well-suited to scenarios where you’re the only person who creates reports, and you don't need to share any data sources with others.

## Download and install a personal mode gateway

  1. [Download the personal mode gateway.](https://go.microsoft.com/fwlink/?LinkId=2116848&clcid=0x409)
  2. In the gateway installer, enter the default installation path, accept the terms of use, and then select Install.

      ![image](https://user-images.githubusercontent.com/20516321/113989982-9d6e2d00-986e-11eb-9961-a3fa02477f21.png)

  3. Enter the email address for your Office 365 organization account, and then select Sign in.
    ![image](https://user-images.githubusercontent.com/20516321/113990054-b1b22a00-986e-11eb-8788-eeb89b005a05.png)

  4. You're now signed in to your account. Select Close.
      ![image](https://user-images.githubusercontent.com/20516321/113990114-c393cd00-986e-11eb-9ac1-ca3a6016a1ed.png)

Reference: 
- https://docs.microsoft.com/en-us/data-integration/gateway/service-gateway-install
- https://docs.microsoft.com/en-us/power-bi/connect-data/refresh-data
- https://docs.microsoft.com/en-us/power-bi/admin/service-premium-incremental-refresh
