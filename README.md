# Get-ODBUsage
.DESCRIPTION  
    Generate a OneDrive for Business Usage report for users  
.PARAMETER AdminSiteUrl  
    Specifies the URL of the SharePoint Online Administration Center site.  
.PARAMETER GlobalAdminUPN  
    Specifies the username of the SharePoint Online global administrator that will be added to the personal sites collection administrators.  
.PARAMETER MySiteHostURL  
    Specifies the location at which the personal sites are created.  
.PARAMETER ImportCSVFile  
    Specify a CSV file with list of users to query for their OD4B sites and get their storage  
.PARAMETER  ExcelFilePath  
    Specifies the path which the report will be stored in. If this parameter is empty, the report will be stored in current directory  
.PARAMETER  FileName  
    Specifies the file name which the report will be. If this parameter is empty, the default name is OneDriveProUsage.csv  
.EXAMPLE  
    .\OD4BUsage.ps1 -AdminSiteUrl https://domain-admin.sharepoint.com -GlobalAdminUPN admin@domain.onmicrosoft.com -MySiteHostURL https://domain-my.sharepoint.com -ImportCSVFile "c:\userslist.csv"  
    .\OD4BUsage.ps1 -AdminSiteUrl https://domain-admin.sharepoint.com -GlobalAdminUPN admin@domain.onmicrosoft.com -MySiteHostURL https://domain-my.sharepoint.com -ExcelFilePath c:\dailyreport -FileName OneDriveProUsage.csv  
