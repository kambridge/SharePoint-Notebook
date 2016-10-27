###Configure claims based authentication
```powershell
$setcba = Get-SPWebApplication "http://YourSiteURL"
$setcba.UseClaimsAuthentication = 1;
$setcba.Update()
```
###Revert back to classic mode authentication (disable Claims Based Authentication)
```powershell
$setcba = Get-SPWebApplication "http://YourSiteURL"
$setcba.UseClaimsAuthentication = 0;
$setcba.Update()
```
