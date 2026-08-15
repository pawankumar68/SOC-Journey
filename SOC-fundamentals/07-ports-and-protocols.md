# 07 – Ports and Protocols

## What is a Protocol?
A protocol is a way of communication — it defines how systems 
connect and communicate with each other to transfer data.

## What is a Port?
Every protocol is given a unique ID called a port number.
Port numbers help identify which service or protocol is being used.

## What is a Socket?
A socket is a combination of IP Address + Port Number.
It identifies a specific connection between two devices.

---

## TCP vs UDP

| TCP | UDP |
|-----|-----|
| Connection based | Connectionless |
| Reliable | Unreliable |
| Slow | Fast |
| Used for web, email | Used for video, gaming, DNS |

---

## TCP Three Way Handshake
1. **SYN** — Client sends synchronize request
2. **SYN + ACK** — Server acknowledges
3. **ACK** — Client confirms connection established

---

## TCP Flags

| Flag | Full Form | Purpose |
|------|-----------|---------|
| SYN | Synchronize | Start connection |
| ACK | Acknowledgement | Confirm data received |
| FIN | Finish | Close connection |
| RST | Reset | Forcefully reset connection |
| PSH | Push | Send data immediately |
| URG | Urgent | Priority data |

SOC Note:
- Many SYN flags = SYN Flood attack 🚩
- Unexpected RST = suspicious forced disconnection
- URG in unusual places = red flag

---

## Common Protocols and Port Numbers

| Protocol | Port | Type | Purpose |
|----------|------|------|---------|
| FTP | 20, 21 | TCP | File transfer (unencrypted) |
| SFTP/SSH | 22 | TCP | Secure file transfer and remote access |
| Telnet | 23 | TCP | Remote access (unencrypted, insecure) |
| SMTP | 25 | TCP | Sending emails |
| DNS | 53 | UDP | Domain to IP resolution |
| DHCP | 67, 68 | UDP | Automatic IP assignment |
| HTTP | 80 | TCP | Web browsing (unencrypted) |
| NTP | 123 | UDP | Network time synchronization |
| HTTPS | 443 | TCP | Secure web browsing (encrypted) |
| RDP | 3389 | TCP | Remote desktop access |

---

## Protocol Categories

### File Transfer Protocols
- **FTP** — Transfers files in plain text, insecure
- **SFTP** — Secure version of FTP, uses encryption
- **TFTP** — Simple file transfer, no authentication

### Email Protocols
- **SMTP** — Sending emails
- **POP3** — Downloads email from server, deletes from server
- **IMAP** — Syncs email, stays on server, multiple device access

### Web Protocols
- **HTTP** — Sends web data in plain text
- **HTTPS** — Encrypts web data using SSL/TLS

### Remote Access Protocols
- **Telnet** — Remote access, plain text, insecure, rarely used today
- **SSH** — Secure remote access using encryption
- **RDP (Port 3389)** — Remote desktop control

### Management Protocols
- **DNS** — Converts domain names to IP addresses
- **DHCP** — Automatically assigns IP addresses to devices
- **NTP** — Synchronizes time across network devices
- **SNMP** — Monitors network devices
- **LDAP/LDAPS** — Directory services, user authentication
- **SMB** — File and printer sharing on Windows networks

---

## Tools to Explore Ports and Protocols

| Tool | Purpose |
|------|---------|
| Nmap | Port and host scanner |
| Wireshark | GUI packet analyzer |
| Netstat | Shows active network connections |
| TCPDump | CLI packet analyzer |

---

## Why This Matters for SOC Analysts
- Every attack uses a protocol and a port
- Unusual port activity = potential threat
- Telnet traffic in modern network = red flag
- Multiple SYN requests = SYN Flood attack
- Suspicious RDP access = possible brute force or unauthorized access
- Phishing emails come through SMTP — monitor SMTP logs
