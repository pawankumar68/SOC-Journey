# What is Networking?

## Room Info
- Path: Pre-Security > Network Fundamentals > What is Networking
- Status: ✅ Completed

## Task 1 — What is Networking?
Networking means connecting two or more systems 
with each other to share information.

## Task 2 — What is the Internet?
The Internet is a Wide Area Network (WAN) that connects 
the entire world.
- First internet was created during the ARPANET project 
  in the 1960s, funded by the US Defence Army
- The modern internet we use today was created in 1989 
  by Tim Berners-Lee with the creation of the World Wide Web
- Internet works on both private and public networks

## Task 3 — Identifying Devices on a Network
Just like a person is identified by their name or fingerprints,
devices on a network are identified by unique identifiers:

- **IP Address** — A virtual address that can change over time
  - No two devices on the same network can have the same IP
  - IPv4 has 4 octets. Example: 192.168.1.1
- **MAC Address** — A unique physical 12 character code
  - Assigned by the network device manufacturer
  - First 6 characters = company that made it
  - Last 6 characters = unique device ID

## Task 4 — Ping (ICMP)
Ping uses the ICMP protocol to measure how long it takes 
to send and receive data from a network device.
It is used to check if a device is reachable on the network.

## How This Connects to Real SOC Work
- IP and MAC addresses are used daily to identify suspicious devices
- Ping is used to check if a suspicious IP is active
- Internet history helps understand how modern attacks evolved
