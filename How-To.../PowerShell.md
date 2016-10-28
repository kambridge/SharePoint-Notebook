__Powershell: Use PowerShell Version 2__
``` 
C:\Windows\System32\WindowsPowerShell\v1.0\PowerShell.exe -Version 2 -NoExit  " & ' C:\Program Files\Common Files\Microsoft Shared\Web Server Extensions\14\CONFIG\POWERSHELL\Registration\\sharepoint.ps1 ' " 
```
__Get Service Application Pool__
```powershell 
Service Application Pool:  Get-SPServiceApplicationPool | select Id, Name 
```
__Start/Stop Timer Service__
```powershell
net stop SPTimerV4
net stop SPAdminV4
```
__Change Usage & Health Data Rentention Policy__
```powershell
Get-SPUsageDefinition | ForEach-Object { if ($_.Enabled -eq “False”) { Set-SPUsageDefinition -Identity $_.Name -DaysRetained 1 }}
```
