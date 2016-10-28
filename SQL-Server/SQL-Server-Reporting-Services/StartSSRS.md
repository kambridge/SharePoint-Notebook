__Start SQL Server Reporting Services:__

1. Install-SPRSService 
2. Install-SPRSServiceProxy 
3. Get/Start Instance
```powershell
Get-SPServiceInstance -all |where {$_.TypeName -like "SQL Server Reporting*"} | Start-SPServiceInstance
```
