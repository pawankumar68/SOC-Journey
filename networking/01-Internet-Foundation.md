# 01 – Internet Fundamentals

This file covers basic networking concepts required to understand how systems communicate over the internet.

---

## OSI Model

The OSI (Open Systems Interconnection) Model is a framework that explains how data travels from one computer to another over a network.

It has 7 layers:

1. Physical – Cables and hardware transmission
2. Data Link – MAC addresses and switching
3. Network – IP addresses and routing
4. Transport – TCP and UDP communication
5. Session – Managing communication sessions
6. Presentation – Data formatting and encryption
7. Application – User-level services like HTTP and DNS

Why It Exists:
To standardize communication between different systems and technologies.

Why Blue Team Cares:
Helps identify at which layer a network issue or attack is occurring.

---

## DNS (Domain Name System)

DNS converts human-readable domain names into IP addresses.

Example:
When you type google.com in your browser,
DNS translates it into an IP address so your system can connect to the correct server.

---

### DNS Record Types
| Record | Purpose | Example |
|--------|---------|---------|
| A | IPv4 address | google.com → 142.x.x.x |
| AAAA | IPv6 address | google.com → 2001:... |
| CNAME | Alias/redirect to another domain | store.google.com → shop.google.com |
| MX | Mail server for the domain | gmail.com mail server |
| TXT | Stores text info, used for verification | SPF, DKIM records |

### How DNS Works (Step by Step)
1. You type **google.com** in browser
2. Your PC checks its **local cache** first
3. If not found → asks **Recursive DNS Resolver** (your ISP)
4. Resolver asks **Root DNS Server** → points to .com server
5. .com server points to **Google's Authoritative DNS**
6. Authoritative DNS returns the IP address
7. Your browser connects to that IP

### Key Terms
- **TTL (Time To Live)** → how long a DNS record is cached (in seconds)
- **Recursive Resolver** → does the lookup work on your behalf
- **Authoritative DNS** → the final source of truth for a domain
- **Root Servers** → top of the DNS hierarchy, 13 sets worldwide

### Blue Team Relevance
- DNS logs help detect **C2 (Command & Control)** malware traffic
- **DNS tunneling** → attackers hide data inside DNS queries
- **DNS spoofing/poisoning** → fake DNS responses redirect users to malicious sites
- Always monitor unusual DNS queries in SOC work