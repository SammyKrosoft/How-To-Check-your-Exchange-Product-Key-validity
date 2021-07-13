# How-To-Check-your-Exchange-Product-Key-validity
Just a very short ReadMe to show you how to test if an Exchange Server Product Key is a valid one

Use the ```[Microsoft.Exchange.Management.SystemConfigurationTasks.ProductKey]``` dotnet notation inside an Exchange Management Shell (or inside a Powershell session where you loaded the local Exchange Management Tools (for example with Get-PSSnapin *Exchange* | Import-PSSnapin, or best, using the Exchange Tools startup lines that you can find on [this article I made specifically for this](https://docs.microsoft.com/en-us/archive/blogs/samdrey/how-to-load-exchange-management-shell-into-powershell-ise-2))

```powershell

$Key5 = "A1B2C3-A1B2C3-A1B2C3-A1B2C3-A1B2C3"

[Microsoft.Exchange.Management.SystemConfigurationTasks.ProductKey]$Key5

```
