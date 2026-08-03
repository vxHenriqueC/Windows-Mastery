# Windows Server

Windows Server is Microsoft's server operating system designed to provide enterprise services such as identity management, file sharing, virtualization, networking, storage, and cloud integration.

---

# Windows Server Roles & Features

| Role / Feature | Description | Category |
|----------------|-------------|----------|
| Active Directory Domain Services (AD DS) | Centralized identity and authentication service. | Identity |
| Active Directory Certificate Services (AD CS) | Public Key Infrastructure (PKI) for issuing digital certificates. | Security |
| Active Directory Federation Services (AD FS) | Single Sign-On (SSO) and federation services. | Identity |
| Active Directory Lightweight Directory Services (AD LDS) | Lightweight LDAP directory service. | Identity |
| DNS Server | Resolves domain names into IP addresses. | Networking |
| DHCP Server | Automatically assigns IP addresses. | Networking |
| File Server | Shares files over the network. | Storage |
| Print Server | Centralized printer management. | Printing |
| Hyper-V | Native virtualization platform. | Virtualization |
| Windows Server Backup | Backup and recovery solution. | Backup |
| Group Policy | Centralized management of Windows settings. | Administration |
| Failover Clustering | Provides high availability between servers. | High Availability |
| IIS | Microsoft web server. | Web |
| Remote Desktop Services | Provides remote desktop sessions. | Remote Access |
| Windows Deployment Services (WDS) | Deploys Windows over the network. | Deployment |
| Storage Spaces Direct | Software-defined storage solution. | Storage |
| Windows Admin Center | Web-based server management tool. | Administration |
| Remote Server Administration Tools (RSAT) | Remote management tools for Windows Server. | Administration |
| Windows Server Update Services (WSUS) | Centralized Windows update management. | Updates |

---

# Common Administration Commands

| Command | Description |
|----------|-------------|
| `sconfig` | Configure Windows Server Core. |
| `dcdiag` | Diagnose Domain Controller health. |
| `repadmin` | Manage Active Directory replication. |
| `gpupdate` | Refresh Group Policies. |
| `gpresult` | Display applied Group Policies. |
| `netdom` | Manage computer/domain relationships. |
| `nltest` | Test secure channels and domain controllers. |
| `w32tm` | Configure Windows Time Service. |
| `wevtutil` | Manage Event Logs. |
| `wbadmin` | Backup and recovery management. |

---

# Common Server Roles

- Domain Controller
- File Server
- Print Server
- DNS Server
- DHCP Server
- Hyper-V Host
- Web Server (IIS)
- Certificate Authority
- VPN Server
- Remote Desktop Server
- Backup Server

---

# Server Editions

| Edition | Usage |
|----------|-------|
| Essentials | Small businesses |
| Standard | Physical and lightly virtualized environments |
| Datacenter | Highly virtualized datacenters |