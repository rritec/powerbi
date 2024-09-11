## Reading Activity

- https://docs.microsoft.com/en-us/learn/modules/introduction-to-powershell/

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
## Exercise 2: Export workspaces/Dashboards/Reports to csv file
-----

1. Click on **New Script** > paste below code and change **workspace id** and **path** accordingly and run it
```
Connect-PowerBIServiceAccount


Get-PowerBIWorkspace | Export-Csv -Path C:\Users\ramreddymyla\Desktop\rritec\20210731\cmdlets\ws.csv
Get-PowerBIDashboard -WorkspaceId 987a132d-795b-406e-9358-b6fbd3fade8f | Export-Csv -Path C:\Users\ramreddymyla\Desktop\rritec\20210731\cmdlets\ds.csv
Get-PowerBIReport -WorkspaceId 987a132d-795b-406e-9358-b6fbd3fade8f | Export-Csv -Path C:\Users\ramreddymyla\Desktop\rritec\20210731\cmdlets\rs.csv
```

## Exercise 3: Get report names from multiple workspaces

   
    $myArray = "9c265642-a2b2-4ae1-a7fe-d9f3822984d7","1083fdff-a6fd-4a92-b849-4387530e8a38"
    #$myArray.Length-1
    $i=0
    for(;$i -le $myArray.Length-1;$i++)
    {
        $myArray[$i]
        Get-PowerBIReport -WorkspaceId $myArray[$i] | Export-Csv -Append -Path C:\work\ps\list_of_sanjay_ws_reports1.csv
    }
    
   
            
### Exercise 4: Get report names from all workspaces

    
      # connect to power BI Service
      Connect-PowerBIServiceAccount


      # Define variables for path and file name
      $path="C:\work\ps\"
      $ws_file_name="list_of_workspaces.csv"
      $rs_file_name="list_of_reports.csv"

      # Export all workspace information
      Get-PowerBIWorkspace | Export-Csv -Path $path$ws_file_name

      # Read csv file of workspaces
      $ws=Import-Csv -Path $path$ws_file_name

      # Read ids of workspaces
      ForEach-Object {
          $Ids += $ws.Id
      }

      # export reportnames from each workspace in append mode

      $i=0
      for(;$i -le $Ids.Length-1;$i++)
      {

          Get-PowerBIReport -WorkspaceId $Ids[$i] | Export-Csv -Append -Path $path$rs_file_name
      }
    
   

## Exercise 5: Create new workspace
-----
```
New-PowerBIWorkspace -Name myla1-workspace
```

## Exercise 6: Remove Power BI Report
----
1. Change report id and workspace id and run it.

```
Remove-PowerBIReport -Id 09d39a15-65ac-46c8-84ac-de2923536cb9 -WorkspaceId 383e66d4-0587-45c8-93dd-0b4a8abec074
```

## Exercise 7: Add/Remove user to/from workspace
----

```
Add-PowerBIWorkspaceUser -Id 79578b7e-3515-421b-bb3f-1fbaee65a319 -UserEmailAddress info@datahexa.com -AccessRight Viewer
Remove-PowerBIWorkspaceUser -Id b901218c-3621-4238-883d-1a7abfdcb58b -UserPrincipalName info@datahexa.com
```
## Exercise 8: Bulk users adding to required workspaces
-----
- Download sample securiy [file](https://github.com/rritec/powerbi/blob/master/Labdata/setup-powerbi-access-to-end-users1.csv) 

      # Define variables for path and file name
      $path="C:\work\ps\"
      $file_name="setup-powerbi-access-to-end-users1.csv"


      # Read csv file of workspaces
      $ws=Import-Csv -Path $path$file_name
      #$ws
      #$Id1=""
      #$UserEmailAddress=""
      #$AccessRights=""

      #Clear-Variable wsId
      #Clear-Variable UserEmailAddress1
      #Clear-Variable AccessRights1

      # Read ids of workspaces
      ForEach-Object {
          $wsId += $ws.workspaceid
          $UserEmailAddress1 += $ws.UserEmailAddress
          $AccessRights1 += $ws.AccessRight   

      }

      # export reportnames from each workspace in append mode

      $i=0
      for(;$i -le $wsId.Length-1;$i++)
      {

          Add-PowerBIWorkspaceUser -Id $wsId[$i] -UserEmailAddress $UserEmailAddress1[$i] -AccessRight $AccessRights1[$i]



      }
      Clear-Variable wsId
      Clear-Variable UserEmailAddress1
      Clear-Variable AccessRights1
## Exercise 9: Disconnect Power BI Service
----

```
Disconnect-PowerBIServiceAccount
```





