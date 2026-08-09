# 05 – OSI and TCP/IP Model

## OSI Model
OSI stands for Open Systems Interconnection.
It is a 7 layer framework that explains how data travels between systems.

### OSI Layers
**Upper Layers (Host Layers):**
- **Layer 7 - Application** — User level services like HTTP, DNS, FTP
- **Layer 6 - Presentation** — Data formatting and encryption
- **Layer 5 - Session** — Managing communication sessions

**Lower Layers (Media Layers):**
- **Layer 4 - Transport** — TCP and UDP communication
- **Layer 3 - Network** — IP addresses and routing
- **Layer 2 - Data Link** — MAC addresses and switching
- **Layer 1 - Physical** — Cables and hardware transmission

---

## OSI Encapsulation and De-encapsulation
- **Encapsulation** — Data gets headers added at each layer as it goes down
- **De-encapsulation** — Headers are removed at each layer as data goes up on receiver side

---

## TCP/IP Model
TCP/IP has 4 layers and is the practical model used in real networks.

| TCP/IP Layer | Protocols |
|-------------|-----------|
| Application | HTTP, DNS, FTP, SMTP |
| Transport | TCP, UDP |
| Internet | IP, ARP, ICMP |
| Network Access | Ethernet, WiFi |

---

## TCP vs UDP
| TCP | UDP |
|-----|-----|
| Connection oriented | Connectionless |
| Reliable, guarantees delivery | Fast but no guarantee |
| Used for web, email | Used for video, gaming, DNS |

---

## MAC Address
- Unique physical address of every network device
- Format: 6 pairs of hexadecimal numbers. Example: 00:1A:2B:3C:4D:5E
- **Windows:** `ipconfig /all`
- **Linux:** `ip a` or `ifconfig`

---

## IP Addresses
- **IPv4** — 32 bit address, ranges from 0-255. Example: 192.168.1.1
- **IPv6** — 128 bit address, created because IPv4 addresses are running out
