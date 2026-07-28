# 💻 Windows Command Prompt (CMD)

The Windows Command Prompt (CMD) is a command-line interpreter used to perform administrative tasks, troubleshoot issues, manage files, configure networks, and automate operations through commands.

---

# 📚 CMD Command Reference

| Command | Description | Category | Admin |
|---------|-------------|----------|:----:|
| `help` | Displays a list of available commands or detailed help for a specific command. | General | ❌ |
| `cls` | Clears the Command Prompt screen. | General | ❌ |
| `exit` | Closes the current Command Prompt session. | General | ❌ |
| `echo` | Displays text or enables/disables command echoing in batch files. | General | ❌ |
| `pause` | Pauses a batch script until a key is pressed. | General | ❌ |
| `title` | Changes the title of the Command Prompt window. | General | ❌ |
| `color` | Changes the text and background colors of the console. | General | ❌ |
| `ver` | Displays the Windows version. | System | ❌ |
| `hostname` | Displays the computer's hostname. | System | ❌ |
| `whoami` | Displays information about the current logged-in user. | System | ❌ |
| `systeminfo` | Displays detailed operating system and hardware information. | System | ❌ |
| `driverquery` | Lists installed device drivers. | System | ❌ |
| `tasklist` | Displays all running processes. | Processes | ❌ |
| `taskkill` | Terminates a process by name or Process ID (PID). | Processes | ✅ |
| `shutdown` | Shuts down, restarts, logs off, or hibernates Windows. | System | ✅ |
| `ipconfig` | Displays and manages the computer's IP configuration. | Networking | ❌ |
| `ipconfig /all` | Shows detailed information for all network adapters. | Networking | ❌ |
| `ipconfig /release` | Releases the current DHCP IP address. | Networking | ✅ |
| `ipconfig /renew` | Requests a new IP address from the DHCP server. | Networking | ✅ |
| `ipconfig /flushdns` | Clears the local DNS resolver cache. | Networking | ✅ |
| `ping` | Tests connectivity to another computer or server using ICMP. | Networking | ❌ |
| `tracert` | Displays the route packets take to reach a destination. | Networking | ❌ |
| `pathping` | Combines ping and tracert to analyze latency and packet loss. | Networking | ❌ |
| `netstat` | Displays active network connections, ports, and statistics. | Networking | ❌ |
| `netsh` | Configures and manages Windows networking settings. | Networking | ✅ |
| `arp` | Displays or modifies the Address Resolution Protocol (ARP) cache. | Networking | ✅ |
| `route` | Displays or modifies the IP routing table. | Networking | ✅ |
| `nslookup` | Queries DNS servers to resolve domain names or IP addresses. | Networking | ❌ |
| `getmac` | Displays the MAC address of network adapters. | Networking | ❌ |
| `net` | Performs various network administration tasks such as managing users, shares, and services. | Administration | ✅ |
| `sc` | Creates, starts, stops, or manages Windows services. | Administration | ✅ |
| `gpresult` | Displays the Group Policy settings applied to a user or computer. | Administration | ❌ |
| `reg` | Creates, edits, deletes, or queries the Windows Registry. | Administration | ✅ |
| `schtasks` | Creates and manages scheduled tasks. | Administration | ✅ |
| `wevtutil` | Manages Windows Event Logs. | Administration | ✅ |
| `logman` | Creates and manages Performance Monitor logs. | Administration | ✅ |
| `sfc /scannow` | Scans and repairs corrupted protected Windows system files. | Maintenance | ✅ |
| `DISM /Online /Cleanup-Image /RestoreHealth` | Repairs the Windows operating system image. | Maintenance | ✅ |
| `chkdsk` | Checks disks for file system errors and bad sectors. | Storage | ✅ |
| `diskpart` | Manages disks, partitions, and volumes. | Storage | ✅ |
| `format` | Formats a storage device with a specified file system. | Storage | ✅ |
| `fsutil` | Performs advanced file system management tasks. | Storage | ✅ |
| `mountvol` | Creates, deletes, or lists volume mount points. | Storage | ✅ |
| `robocopy` | Copies files and directories with advanced synchronization options. | File Management | ❌ |
| `xcopy` | Copies files and directory trees. | File Management | ❌ |
| `copy` | Copies one or more files. | File Management | ❌ |
| `move` | Moves files or folders to another location. | File Management | ❌ |
| `del` | Deletes one or more files. | File Management | ❌ |
| `erase` | Deletes files (alias for `del`). | File Management | ❌ |
| `mkdir` | Creates a new directory. | File Management | ❌ |
| `rmdir` | Removes an empty directory or directory tree. | File Management | ❌ |
| `ren` | Renames files or directories. | File Management | ❌ |
| `tree` | Displays the directory structure in a tree format. | File Management | ❌ |
| `attrib` | Displays or changes file and folder attributes. | File Management | ❌ |
| `takeown` | Takes ownership of files or folders. | Security | ✅ |
| `icacls` | Displays or modifies NTFS permissions. | Security | ✅ |
| `cipher` | Manages NTFS file encryption. | Security | ✅ |
| `manage-bde` | Manages BitLocker Drive Encryption. | Security | ✅ |
| `certutil` | Manages certificates and performs encoding, decoding, and hashing operations. | Security | ✅ |
| `bcdedit` | Displays or edits the Boot Configuration Data (BCD). | Boot | ✅ |
| `bootrec` | Repairs the Windows boot environment. | Boot | ✅ |
| `reagentc` | Configures the Windows Recovery Environment (WinRE). | Recovery | ✅ |