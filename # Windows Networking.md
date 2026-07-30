#  Windows Networking

This document explains the main networking concepts, protocols, services, and tools used in Microsoft Windows environments. It also includes common Windows commands for diagnosing and troubleshooting network issues.

---

#  Networking Reference

| Technology | Description | Category | Windows Support |
|------------|-------------|----------|-----------------|
| TCP | Connection-oriented protocol that provides reliable data transmission. | Protocol | ✅ |
| UDP | Connectionless protocol used for fast communication with low overhead. | Protocol | ✅ |
| IP | Protocol responsible for addressing and routing packets between devices. | Protocol | ✅ |
| IPv4 | 32-bit addressing protocol used by most networks today. | Protocol | ✅ |
| IPv6 | 128-bit addressing protocol designed to replace IPv4. | Protocol | ✅ |
| ICMP | Protocol used for diagnostics and error reporting (Ping, Tracert). | Protocol | ✅ |
| ARP | Resolves IPv4 addresses into MAC addresses on local networks. | Protocol | ✅ |
| DNS | Translates domain names into IP addresses. | Service | ✅ |
| DHCP | Automatically assigns IP addresses and network settings. | Service | ✅ |
| NAT | Translates private IP addresses into public IP addresses. | Networking | ✅ |
| Gateway | Device that routes traffic between different networks. | Networking | ✅ |
| Subnet Mask | Defines the network and host portions of an IP address. | Addressing | ✅ |
| CIDR | Classless addressing notation for IP networks. | Addressing | ✅ |
| MAC Address | Unique hardware identifier assigned to a network adapter. | Hardware | ✅ |
| Default Gateway | Router used to reach external networks. | Routing | ✅ |
| Routing Table | Stores routes used to forward network traffic. | Routing | ✅ |
| VLAN | Creates logical network segments within the same physical infrastructure. | Networking | Depends on Hardware |
| VPN | Creates an encrypted tunnel between devices over the Internet. | Security | ✅ |
| Proxy | Intermediary server between a client and the destination. | Networking | ✅ |
| Firewall | Filters incoming and outgoing network traffic. | Security | ✅ |
| SMB | Windows protocol for file and printer sharing. | File Sharing | ✅ |
| NetBIOS | Legacy protocol for communication on Windows networks. | Legacy | ✅ |
| LDAP | Directory access protocol used by Active Directory. | Directory Services | Windows Server |
| Kerberos | Authentication protocol used in Active Directory. | Authentication | Windows Server |
| RDP | Remote Desktop Protocol for remote computer access. | Remote Access | Pro/Enterprise |
| SSH | Secure protocol for remote command-line access. | Remote Access | Windows 10+ |
| FTP | Protocol used to transfer files over a network. | File Transfer | Optional |
| SFTP | Secure file transfer protocol over SSH. | File Transfer | Optional |
| HTTP | Protocol used to transfer web pages. | Web | ✅ |
| HTTPS | Secure version of HTTP using TLS encryption. | Web | ✅ |
| TLS | Cryptographic protocol protecting network communications. | Security | ✅ |
| DNS Cache | Local storage of recently resolved DNS queries. | DNS | ✅ |
| Hosts File | Local file used to manually resolve hostnames. | DNS | ✅ |
| Loopback Address | Reserved IP used for testing the local machine (`127.0.0.1`). | Addressing | ✅ |
| APIPA | Automatic private IP assigned when DHCP is unavailable (`169.254.x.x`). | Addressing | ✅ |

---

#  Windows Networking Commands

| Command | Description |
|----------|-------------|
| `ipconfig` | Displays and manages IP configuration. |
| `ping` | Tests connectivity with another host. |
| `tracert` | Displays the route packets take to a destination. |
| `pathping` | Combines Ping and Tracert for network diagnostics. |
| `netstat` | Displays active connections, ports, and statistics. |
| `arp` | Displays or modifies the ARP cache. |
| `route` | Displays or modifies the routing table. |
| `hostname` | Displays the computer name. |
| `nslookup` | Queries DNS servers. |
| `netsh` | Configures Windows networking. |
| `getmac` | Displays MAC addresses. |
| `Test-NetConnection` | Tests ports and connectivity (PowerShell). |
| `Resolve-DnsName` | Queries DNS records (PowerShell). |

---

#  Common Ports

| Port | Protocol | Service |
|------|----------|---------|
| 20/21 | TCP | FTP |
| 22 | TCP | SSH |
| 23 | TCP | Telnet |
| 25 | TCP | SMTP |
| 53 | TCP/UDP | DNS |
| 67/68 | UDP | DHCP |
| 69 | UDP | TFTP |
| 80 | TCP | HTTP |
| 110 | TCP | POP3 |
| 123 | UDP | NTP |
| 143 | TCP | IMAP |
| 161 | UDP | SNMP |
| 389 | TCP/UDP | LDAP |
| 443 | TCP | HTTPS |
| 445 | TCP | SMB |
| 3389 | TCP | Remote Desktop (RDP) |

---

# Network Troubleshooting Workflow

1. Check the network adapter.
2. Verify the IP address (`ipconfig`).
3. Test the loopback address (`127.0.0.1`).
4. Ping the default gateway.
5. Ping another device on the LAN.
6. Test Internet connectivity.
7. Verify DNS resolution.
8. Inspect active connections (`netstat`).
9. Review the routing table (`route print`).
10. Check Windows Firewall rules.

---

#  Quick Tips

- `127.0.0.1` → Localhost (Loopback)
- `0.0.0.0` → Default route / Any address
- `169.254.x.x` → APIPA (DHCP failure)
- `255.255.255.255` → Broadcast address
- `::1` → IPv6 Loopback
- Private IPv4 ranges:
  - `10.0.0.0/8`
  - `172.16.0.0/12`
  - `192.168.0.0/16`