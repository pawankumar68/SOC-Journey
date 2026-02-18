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

Why DNS Is Important:
Without DNS, users would need to remember IP addresses instead of domain names.

Why Blue Team Cares:
DNS logs help detect suspicious activity such as malware communication or unusual domain lookups.

