# Intro to LAN

## Room Info
- Path: Pre-Security > Network Fundamentals > Intro to LAN
- Status: ✅ Completed

## Task 1 — LAN Topologies
Topology means the design of a network connection.
3 types of topologies:

- **Star** — All devices connected to one central router/switch
  - Most expensive topology
  - If central device fails, entire network stops
- **Bus** — All devices connected to one single backbone cable
  - Cheapest topology
  - Data passes through all devices = delay and data theft risk
- **Ring (Circle)** — Every device connected to 2 other devices forming a circle
  - If the circle is damaged, data sharing stops

## Task 2 — Subnetting
Subnetting means dividing one large network into smaller multiple networks.
- Range: 0-255
- For small networks like home, one subnet is enough
  because rarely 254 devices connect at once
- Subnetting uses IP address in 3 ways:
  - **Network Address** — Identifies the network
  - **Host Address** — Identifies the device
  - **Default Gateway** — Device that sends data outside the network

## Task 3 — ARP (Address Resolution Protocol)
ARP helps devices identify themselves on a network.
Every device has 2 identifiers — MAC address and IP address.

How ARP works:
1. Device wants to communicate with another device
2. Sends a **ARP Request** (broadcast) — "Which MAC address has this IP?"
3. The device with that IP responds with **ARP Reply**
4. This info gets stored in **ARP Cache** for future communication

## Task 4 — DHCP (Dynamic Host Configuration Protocol)
IP address is assigned to a device in 2 ways — manually or automatically.
DHCP is the most commonly used automatic method.

How DHCP works:
1. Device connects to network without a manual IP
2. Sends a **DHCP Discover** request
3. DHCP server **Offers** an IP address
4. Device **Accepts** the offer
5. DHCP sends **ACK** — IP assigned for 24 hours

## How This Connects to Real SOC Work
- ARP Cache poisoning is a common attack — SOC analysts monitor ARP traffic
- DHCP Starvation is a network attack — understanding DHCP helps detect it
- Subnetting helps analysts identify which network segment an attack came from
