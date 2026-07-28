# ⚡ Windows PowerShell

PowerShell is Microsoft's command-line shell and scripting language designed for system administration, automation, and configuration management. Unlike Command Prompt (CMD), PowerShell works with **objects** instead of plain text, making it significantly more powerful for managing Windows systems.

---

# 📚 PowerShell Command Reference

| Command | Description | Category | Admin |
|---------|-------------|:--------:|:----:|
| `Get-Help` | Displays help information for commands and cmdlets. | Help | ❌ |
| `Update-Help` | Downloads and updates PowerShell help files. | Help | ✅ |
| `Get-Command` | Lists all available PowerShell commands, functions, aliases, and scripts. | Help | ❌ |
| `Get-Alias` | Displays all PowerShell aliases. | Help | ❌ |
| `Get-History` | Shows previously executed commands. | General | ❌ |
| `Clear-History` | Clears the PowerShell command history. | General | ❌ |
| `Get-Location` | Displays the current working directory. | File System | ❌ |
| `Set-Location` | Changes the current working directory. | File System | ❌ |
| `Get-ChildItem` | Lists files and folders in a directory. | File System | ❌ |
| `New-Item` | Creates a new file, folder, registry key, or other object. | File System | ❌ |
| `Copy-Item` | Copies files, folders, or other items. | File System | ❌ |
| `Move-Item` | Moves files or folders. | File System | ❌ |
| `Rename-Item` | Renames files or folders. | File System | ❌ |
| `Remove-Item` | Deletes files, folders, or other objects. | File System | ❌ |
| `Get-Content` | Reads the contents of a file. | File System | ❌ |
| `Set-Content` | Replaces the contents of a file. | File System | ❌ |
| `Add-Content` | Appends content to a file. | File System | ❌ |
| `Clear-Content` | Removes the contents of a file while keeping the file. | File System | ❌ |
| `Test-Path` | Checks whether a path exists. | File System | ❌ |
| `Resolve-Path` | Resolves the full path of a file or directory. | File System | ❌ |
| `Get-Process` | Lists running processes. | Processes | ❌ |
| `Start-Process` | Starts a new process or application. | Processes | ❌ |
| `Stop-Process` | Stops a running process. | Processes | ✅ |
| `Wait-Process` | Waits for a process to finish. | Processes | ❌ |
| `Get-Service` | Lists Windows services. | Services | ❌ |
| `Start-Service` | Starts a Windows service. | Services | ✅ |
| `Stop-Service` | Stops a Windows service. | Services | ✅ |
| `Restart-Service` | Restarts a Windows service. | Services | ✅ |
| `Set-Service` | Changes service properties. | Services | ✅ |
| `Get-ComputerInfo` | Displays detailed system information. | System | ❌ |
| `Get-CimInstance` | Retrieves management information using CIM. | System | ❌ |
| `Get-WmiObject` | Retrieves management information using WMI (legacy). | System | ❌ |
| `Get-EventLog` | Displays Windows Event Logs (legacy). | System | ❌ |
| `Get-WinEvent` | Reads Windows Event Logs. | System | ❌ |
| `Restart-Computer` | Restarts the computer. | System | ✅ |
| `Stop-Computer` | Shuts down the computer. | System | ✅ |
| `Test-Connection` | Tests network connectivity using ICMP. | Networking | ❌ |
| `Test-NetConnection` | Tests TCP ports, DNS, and network connectivity. | Networking | ❌ |
| `Get-NetIPAddress` | Displays IP address configuration. | Networking | ❌ |
| `Get-NetAdapter` | Displays installed network adapters. | Networking | ❌ |
| `Enable-NetAdapter` | Enables a network adapter. | Networking | ✅ |
| `Disable-NetAdapter` | Disables a network adapter. | Networking | ✅ |
| `Resolve-DnsName` | Resolves DNS records. | Networking | ❌ |
| `Get-DnsClientCache` | Displays the DNS cache. | Networking | ❌ |
| `Clear-DnsClientCache` | Clears the DNS cache. | Networking | ✅ |
| `Invoke-WebRequest` | Sends HTTP/HTTPS requests and downloads web content. | Networking | ❌ |
| `Invoke-RestMethod` | Sends REST API requests and automatically parses responses. | Networking | ❌ |
| `Enter-PSSession` | Opens an interactive remote PowerShell session. | Remote Management | ❌ |
| `Exit-PSSession` | Closes a remote PowerShell session. | Remote Management | ❌ |
| `Invoke-Command` | Executes commands on local or remote computers. | Remote Management | ❌ |
| `New-PSSession` | Creates a persistent remote PowerShell session. | Remote Management | ❌ |
| `Remove-PSSession` | Closes a remote PowerShell session. | Remote Management | ❌ |
| `Get-ExecutionPolicy` | Displays the current PowerShell execution policy. | Security | ❌ |
| `Set-ExecutionPolicy` | Changes the PowerShell execution policy. | Security | ✅ |
| `Get-LocalUser` | Lists local user accounts. | Users | ✅ |
| `New-LocalUser` | Creates a local user account. | Users | ✅ |
| `Remove-LocalUser` | Deletes a local user account. | Users | ✅ |
| `Add-LocalGroupMember` | Adds a user to a local group. | Users | ✅ |
| `Get-LocalGroupMember` | Lists members of a local group. | Users | ✅ |
| `Get-Disk` | Lists physical disks. | Storage | ❌ |
| `Get-Partition` | Lists disk partitions. | Storage | ❌ |
| `Get-Volume` | Lists storage volumes. | Storage | ❌ |
| `Get-PSDrive` | Lists available PowerShell drives. | Storage | ❌ |
| `Get-Date` | Displays the current date and time. | Utility | ❌ |
| `Measure-Object` | Calculates count, average, sum, minimum, and maximum values. | Utility | ❌ |
| `Select-Object` | Selects specific properties from objects. | Utility | ❌ |
| `Sort-Object` | Sorts objects. | Utility | ❌ |
| `Where-Object` | Filters objects based on conditions. | Utility | ❌ |
| `ForEach-Object` | Executes an action for each object in a collection. | Utility | ❌ |
| `Compare-Object` | Compares two sets of objects. | Utility | ❌ |
| `Export-CSV` | Exports objects to a CSV file. | Utility | ❌ |
| `Import-CSV` | Imports objects from a CSV file. | Utility | ❌ |
| `ConvertTo-Json` | Converts objects into JSON format. | Utility | ❌ |
| `ConvertFrom-Json` | Converts JSON into PowerShell objects. | Utility | ❌ |
| `Out-File` | Sends output to a file. | Utility | ❌ |
| `Write-Host` | Displays text on the console. | Utility | ❌ |