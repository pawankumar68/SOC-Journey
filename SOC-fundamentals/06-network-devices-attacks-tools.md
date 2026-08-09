# 06 – Network Devices, Attacks and SOC Tools

## Network Topologies

### Wired Topologies
- **Bus** — Sabhi devices ek single cable se connected, ek fail sab fail
- **Ring** — Devices ring mein connected, data ek direction mein travel karta hai
- **Star** — Sabhi devices central switch se connected, most common
- **Mesh** — Har device har doosre se connected, most reliable

### Wireless Topologies
- **Ad Hoc** — Direct device to device, no central access point
- **Infrastructure** — Devices WAP ke through connect hote hain
- **Mesh** — Multiple WAPs connected for wide coverage

---

## Networking Protocols
- **Physical Protocols** — Hardware level communication rules. Example: Ethernet, WiFi
- **Logical Protocols** — Software level rules. Example: TCP/IP, HTTP, DNS
## Network Devices
- **NIC (Network Interface Card)** — Hardware that connects device to network
- **Hub** — Sends data to all devices on network, not smart
- **Switch** — Sends data only to target device, smarter than hub
- **Router** — Connects different networks together
- **Modem** — Converts digital signal to analog and back for internet
- **WAP (Wireless Access Point)** — Provides WiFi connectivity
- **Firewall** — Monitors and filters network traffic based on rules
- **DHCP Server** — Automatically assigns IP addresses to devices
- **Media Converter** — Converts one type of cable signal to another
- **SOHO Device** — Small Office Home Office device, combines router, switch, WAP
- **VoIP Endpoint** — Device used for voice calls over internet

---

## Network Cables
- **Coaxial** — Old cable type, used in cable TV
- **Twisted Pair** — Most common, used in LAN. Example: Ethernet cable
- **Fiber Optic** — Fastest, uses light to transmit data, used for long distances

---

## Common Network Based Attacks
- **MITM (Man in the Middle)** — Attacker sits between two parties and intercepts communication
- **DNS Spoofing** — Fake DNS response to redirect user to malicious site
- **ARP Spoofing** — Fake ARP messages to link attacker MAC with victim IP
- **SYN Flood** — Attacker sends many SYN requests to overwhelm server
- **DHCP Starvation** — Attacker exhausts all DHCP IP addresses so no device gets IP
- **Packet Sniffing** — Capturing network traffic to steal data
- **Port Scanning** — Scanning open ports to find vulnerabilities

---

## SOC Tools for Network Analysis
| Tool | Type | Purpose |
|------|------|---------|
| Wireshark | GUI | Packet sniffer and analyzer |
| TCPDump | CLI | Command line packet analyzer |
| Netstat | CLI | Shows active network connections |
| Nmap | CLI | Port and host scanner |
| NSLookup | CLI | DNS lookup tool |
| MTR | CLI | Path and route scanner |

---

## Common Protocols and Port Numbers
| Protocol | Port |
|----------|------|
| HTTP | 80 |
| HTTPS | 443 |
| FTP | 21 |
| SSH | 22 |
| DNS | 53 |
| SMTP | 25 |
| RDP | 3389 |

---

## ARP (Address Resolution Protocol)
- Converts IP address to MAC address
- Used when device knows IP but needs MAC to communicate on local network
