# 08 – IP Addressing

## What is an IP Address?
An IP address is a unique identifier for a device to communicate
on the internet. It can be public or private.
There are two types: IPv4 and IPv6.

---

## IPv4 vs IPv6

| Feature | IPv4 | IPv6 |
|---------|------|------|
| Bits | 32 bits | 128 bits |
| Format | 4 octets (decimal) | 8 groups (hexadecimal) |
| Example | 192.168.1.1 | 2001:0db8:85a3::8a2e:0370:7334 |
| Total Addresses | 4.3 billion | Virtually unlimited |
| Why Created | Original design | IPv4 addresses running out |

---

## IPv4 Address Classes

| Class | Network Bits | Host Bits | Range |
|-------|-------------|-----------|-------|
| A | 8 | 24 | 1.0.0.0 – 126.255.255.255 |
| B | 16 | 16 | 128.0.0.0 – 191.255.255.255 |
| C | 24 | 8 | 192.0.0.0 – 223.255.255.255 |
| D | — | — | 224.0.0.0 – 239.255.255.255 (Multicast) |
| E | — | — | 240.0.0.0 – 255.255.255.255 (Research) |

---

## Public vs Private IP

| Public IP | Private IP |
|-----------|------------|
| Routable on internet | Used inside LAN only |
| Assigned by ISP | Unregistered, free to use |
| Must be globally unique | Can be reused anywhere |
| Used by web servers, DNS, routers | Used inside home/office networks |
| Registered IP address | Anyone can use |

### Private IP Ranges
| Class | Range |
|-------|-------|
| A | 10.0.0.0 – 10.255.255.255 |
| B | 172.16.0.0 – 172.31.255.255 |
| C | 192.168.0.0 – 192.168.255.255 |

---

## Subnetting Basics
Dividing a large network into smaller logical networks
based on subnet mask (e.g. /24, /26).

## CIDR Notation
CIDR = Classless Inter-Domain Routing
Example: 192.168.1.0/24
- /24 means 24 bits are network bits
- Subnet mask = 255.255.255.0

---

## Loopback Address
- Reserved address for host's own communication
- Also called localhost or local address
- Used to check if TCP/IP is correctly installed in OS
- Range: 127.0.0.0 – 127.255.255.255
- Default: **127.0.0.1**

---

## Tools to Check IP

| Tool | Platform | Purpose |
|------|----------|---------|
| ipconfig | Windows | Check IP address |
| ip a / ifconfig | Linux | Check IP address |
| checkmyip.com | Web | Check public IP |

---

## IP Addressing in SOC
- **Log Analysis** — IP addresses in logs identify source of traffic
- **Identifying Attack Sources** — Trace malicious IPs
- **Firewall Rules** — Block suspicious IPs
- **Network Segmentation Monitoring** — Monitor traffic between segments

> 💡 SOC tools like SIEMs rely heavily on IP data for correlation
> of events across multiple systems.
