# Power BI Cmdlets for Windows PowerShell and PowerShell Core
https://docs.microsoft.com/en-us/powershell/power-bi/overview?view=powerbi-ps

## Exercise 1: Install all modules of PowerBI
-----
1. Open **Windows PowerShell ISE(X86)** > In power Shell window run below command
```
Install-Module -Name MicrosoftPowerBIMgmt
```
2. In right side **Commands** window click on refresh observe all **six** useful modules are installed.
```

MicrosoftPowerBIMgmt.Admin
MicrosoftPowerBIMgmt.Capacities
MicrosoftPowerBIMgmt.Data
MicrosoftPowerBIMgmt.Profile
MicrosoftPowerBIMgmt.Reports
MicrosoftPowerBIMgmt.Workspaces
```
## Exercise 2: Export workspaces to csv file
-----

1. Click on **New Script** > paste below code and change path accordingly and run it
```
Connect-PowerBIServiceAccount

Get-PowerBIWorkspace | Export-Csv -Path C:\work\powerbi-powershell\ws.csv
```

## Exercise 3: Create new workspace
-----
```
New-PowerBIWorkspace -Name myla1-workspace
```

## Exercise 4: Remove Power BI Report
----
1. Change report id and workspace id and run it.
```
Remove-PowerBIReport -Id 09d39a15-65ac-46c8-84ac-de2923536cb9 -WorkspaceId 383e66d4-0587-45c8-93dd-0b4a8abec074
```

## Exercise 5: disconnect Power BI Service
----
```
Disconnect-PowerBIServiceAccount
```





