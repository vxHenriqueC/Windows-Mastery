# Active Directory

Active Directory (AD) is Microsoft's directory service used to manage users, computers, groups, permissions, and authentication within Windows domains.

---

# Active Directory Components

| Component | Description |
|-----------|-------------|
| Domain | Logical collection of users, computers, and resources. |
| Forest | Collection of one or more domains. |
| Tree | Hierarchical collection of domains. |
| Organizational Unit (OU) | Container used to organize objects. |
| Domain Controller (DC) | Server hosting Active Directory services. |
| Global Catalog | Stores searchable information from the forest. |
| Schema | Defines object classes and attributes. |
| Sites | Represents physical network locations. |
| Trust | Relationship between domains or forests. |

---

# Active Directory Objects

| Object | Description |
|---------|-------------|
| User | Represents a person or service account. |
| Computer | Represents a joined device. |
| Group | Collection of users or computers. |
| Contact | Stores contact information. |
| Printer | Shared printer object. |
| Shared Folder | Network shared resource. |

---

# Authentication

| Technology | Description |
|------------|-------------|
| Kerberos | Default authentication protocol. |
| NTLM | Legacy authentication protocol. |
| LDAP | Directory access protocol. |
| LDAPS | Secure LDAP over SSL/TLS. |

---

# Common Active Directory Commands

| Command | Description |
|----------|-------------|
| `dsquery` | Search Active Directory objects. |
| `dsadd` | Create Active Directory objects. |
| `dsmod` | Modify Active Directory objects. |
| `dsrm` | Remove Active Directory objects. |
| `dsmove` | Move Active Directory objects. |
| `net user` | Manage users. |
| `net group` | Manage groups. |
| `gpupdate` | Refresh Group Policies. |
| `gpresult` | Display applied Group Policies. |
| `dcdiag` | Diagnose Domain Controllers. |
| `repadmin` | Check replication status. |
| `nltest` | Test trust relationships. |

---

# Group Policy

Group Policy allows administrators to configure Windows settings centrally.

Examples:

- Password Policy
- Account Lockout Policy
- USB Restrictions
- Windows Update
- Desktop Restrictions
- Firewall Rules
- Login Scripts
- Drive Mapping

---

# Active Directory Structure

```text
Forest
└── Domain
    ├── Domain Controllers
    ├── Users
    ├── Computers
    ├── Groups
    ├── Servers
    ├── Workstations
    └── Organizational Units (OUs)
```

---

# FSMO Roles

| Role | Purpose |
|------|---------|
| Schema Master | Controls schema changes. |
| Domain Naming Master | Manages domains in the forest. |
| RID Master | Allocates Relative IDs. |
| PDC Emulator | Password changes and time synchronization. |
| Infrastructure Master | Updates object references between domains. |

---

# Best Practices

- Use Organizational Units (OUs).
- Apply least privilege.
- Use Group Policies instead of manual configuration.
- Monitor replication.
- Secure privileged accounts.
- Back up Domain Controllers regularly.
- Enable auditing.
- Use strong password policies.
- Implement Multi-Factor Authentication where possible.