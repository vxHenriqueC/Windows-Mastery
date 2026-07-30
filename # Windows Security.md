#  Windows Security

This document provides an overview of the most important security technologies, tools, and features available in Microsoft Windows. It covers authentication, encryption, malware protection, access control, and system hardening.

---

#  Security Reference

| Feature | Description | Category | Available |
|---------|-------------|----------|-----------|
| Microsoft Defender Antivirus | Built-in antivirus that protects against malware, ransomware, and other threats. | Antivirus | Windows 10+ |
| Microsoft Defender Firewall | Monitors and filters inbound and outbound network traffic. | Firewall | All |
| BitLocker | Encrypts entire drives to protect data if a device is lost or stolen. | Encryption | Pro / Enterprise |
| BitLocker To Go | Encrypts removable USB drives and external storage devices. | Encryption | Pro / Enterprise |
| TPM (Trusted Platform Module) | Hardware security chip used for encryption keys, BitLocker, and Windows Hello. | Hardware Security | Modern PCs |
| Secure Boot | Prevents unauthorized operating systems and bootloaders from loading during startup. | Boot Security | UEFI Systems |
| Windows Hello | Passwordless authentication using PIN, fingerprint, or facial recognition. | Authentication | Windows 10+ |
| Credential Manager | Securely stores usernames, passwords, and certificates. | Credentials | All |
| SmartScreen | Protects users from malicious websites, downloads, and applications. | Web Protection | Windows 8+ |
| User Account Control (UAC) | Prompts for administrator approval before privileged actions. | Privilege Management | All |
| Windows Security | Central application for managing Windows security features. | Security Center | Windows 10+ |
| Device Encryption | Automatic encryption available on supported devices. | Encryption | Supported Devices |
| Windows Sandbox | Runs applications in an isolated temporary environment. | Isolation | Pro / Enterprise |
| Microsoft Defender Smart App Control | Blocks untrusted or unsigned applications. | Application Control | Windows 11 |
| AppLocker | Restricts which applications users can execute. | Application Control | Enterprise / Education |
| Windows Defender Application Control (WDAC) | Controls which applications and drivers are allowed to run. | Application Control | Enterprise |
| Exploit Protection | Protects applications against memory-based attacks. | Exploit Mitigation | Windows 10+ |
| Controlled Folder Access | Prevents ransomware from modifying protected folders. | Ransomware Protection | Windows 10+ |
| Windows Defender Credential Guard | Protects credentials using virtualization-based security. | Credential Protection | Enterprise |
| Windows Defender Application Guard | Isolates Microsoft Edge sessions from the operating system. | Browser Security | Enterprise |
| Local Security Policy | Configures password, audit, and security policies. | Administration | Pro / Enterprise |
| Group Policy | Centrally manages Windows security settings. | Administration | Pro / Enterprise |
| Windows Update | Installs security patches and system updates. | Maintenance | All |
| Event Viewer | Displays security, application, and system logs. | Monitoring | All |
| Audit Policy | Records security events such as logons and object access. | Auditing | Pro / Enterprise |
| NTFS Permissions | Controls access to files and folders using Access Control Lists (ACLs). | File Security | All |
| EFS (Encrypting File System) | Encrypts individual files and folders on NTFS volumes. | Encryption | Pro / Enterprise |
| Remote Desktop (RDP) | Allows secure remote access to Windows computers. | Remote Access | Pro / Enterprise |
| Windows LAPS | Automatically manages local administrator passwords. | Password Management | Windows 11 / Windows Server |

---

#  Security Commands

| Command | Description |
|----------|-------------|
| `manage-bde` | Manage BitLocker encryption. |
| `cipher` | Encrypt or decrypt files using EFS. |
| `icacls` | Display or modify NTFS permissions. |
| `takeown` | Take ownership of files and folders. |
| `whoami` | Display the current user and security information. |
| `gpresult` | Display applied Group Policies. |
| `gpupdate` | Refresh Group Policy settings. |
| `auditpol` | Configure and display audit policies. |
| `net user` | Manage local user accounts. |
| `net localgroup` | Manage local security groups. |
| `runas` | Execute a program as another user. |
| `certutil` | Manage certificates and perform cryptographic operations. |
| `wevtutil` | Manage Windows Event Logs. |
| `sfc /scannow` | Scan and repair protected Windows system files. |
| `DISM /Online /Cleanup-Image /RestoreHealth` | Repair the Windows system image. |

---

#  Authentication Methods

| Method | Description |
|---------|-------------|
| Password | Traditional user authentication method. |
| PIN | Device-specific authentication used by Windows Hello. |
| Fingerprint | Biometric authentication. |
| Facial Recognition | Windows Hello Face authentication. |
| Smart Card | Authentication using physical security cards. |
| FIDO2 Security Key | Passwordless authentication using hardware security keys. |

---

#  Security Best Practices

- Keep Windows Update enabled.
- Enable BitLocker on supported devices.
- Use Microsoft Defender Antivirus.
- Enable Microsoft Defender Firewall.
- Use strong, unique passwords.
- Enable Multi-Factor Authentication (MFA) whenever possible.
- Avoid running as a local administrator for daily tasks.
- Keep applications updated.
- Regularly back up important files.
- Monitor Event Viewer for security-related events.

---

#  Common Security Threats

| Threat | Description |
|--------|-------------|
| Malware | Software designed to damage or compromise systems. |
| Ransomware | Encrypts files and demands payment for recovery. |
| Phishing | Attempts to steal credentials through deceptive messages. |
| Brute Force | Repeated login attempts to guess passwords. |
| Privilege Escalation | Gaining unauthorized administrative privileges. |
| Rootkit | Malware designed to hide itself and other malicious software. |
| Spyware | Secretly collects user information. |
| Keylogger | Records keyboard input to steal credentials. |
| Zero-Day | Exploit targeting a vulnerability before a patch is available. |
| Social Engineering | Manipulating users into revealing sensitive information. |

---

# Security Checklist

- ✅ Windows Defender enabled
- ✅ Firewall enabled
- ✅ BitLocker enabled
- ✅ Secure Boot enabled
- ✅ TPM available
- ✅ Windows Update enabled
- ✅ Strong password or Windows Hello configured
- ✅ Backup configured
- ✅ Recovery options available
- ✅ Event logs monitored