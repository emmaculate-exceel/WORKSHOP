I was able to fix the problem by going to the windows powershell and run it as an admin
then use the below code

Get-AppXPackage *WindowsStore* -AllUsers | Foreach {Add-AppxPackage -DisableDevelopmentMode -Register "$($_.InstallLocation)\AppXManifest.xml"}

and the issue was resolved .