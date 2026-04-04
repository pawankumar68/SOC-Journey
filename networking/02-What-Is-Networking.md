# What is Networking
*Source: TryHackMe — "What is Networking" room*

---

## 1. What is Networking?
- A network is when two or more devices are connected to share data/resources
- Networks can be as small as 2 computers at home or as large as the internet
- Networks allow devices to communicate with each other

---

## 2. What is the Internet?
- The internet is one giant network made up of millions of smaller networks
- It consists of private and public networks connected together
- ARPANET (1960s) was the first version of the internet, funded by the US military
- Tim Berners-Lee invented the World Wide Web (WWW) in 1989

---

## 3. Identifying Devices on a Network
Two main ways devices are identified:

### IP Address (Internet Protocol)
- A logical address assigned to a device on a network
- Can change when you join a different network
- Two versions:
  - **IPv4** → 32-bit → Example: 192.168.1.1 (about 4.29 billion addresses)
  - **IPv6** → 128-bit → Example: 2001:0db8:85a3:0000:0000:8a2e:0370:7334 (virtually unlimited)

### MAC Address (Media Access Control)
- A physical/hardware address burned into the network card (NIC)
- Permanent and unique to each device
- Format: 6 pairs of hex digits → Example: a4:c3:f0:85:ac:2d
- First 3 pairs = manufacturer, Last 3 pairs = unique device ID
- Can be spoofed (faked) by attackers — important for Blue Team awareness

---

## 4. Ping (ICMP)
- Ping uses **ICMP (Internet Control Message Protocol)** to test connectivity
- It checks if a device is reachable and measures response time
- Works by sending an **ICMP Echo Request** and waiting for an **ICMP Echo Reply**
- Measured in milliseconds (ms)

### Basic usage:
```bash
ping <ip-address>       # ping by IP
ping <domain-name>      # ping by domain e.g. ping google.com
ping -c 4 google.com    # send only 4 packets (Linux)
```

### Blue Team relevance:
- Attackers use ping to discover live hosts on a network (reconnaissance)
- Many firewalls block ICMP to prevent this
- No reply doesn't always mean the host is down — it may just block ping

---

## Key Takeaways
- Every device on a network needs an IP (logical) and MAC (physical) address
- IPv6 was created because IPv4 addresses are running out
- Ping is the simplest way to test if a device is online
- MAC addresses can be spoofed — never fully trust them for authentication