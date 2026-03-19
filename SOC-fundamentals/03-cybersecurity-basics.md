# 03 – Cybersecurity Basics
 
---
 
## What is Cybersecurity?
Cybersecurity is the practice of protecting systems, networks, and data from digital attacks,
unauthorized access, damage, or theft.
 
---
 
## Why is Cybersecurity Important?
- Protects sensitive data (personal, financial, organizational)
- Prevents financial losses from attacks
- Maintains trust in digital systems
- Ensures business continuity
- Required for compliance (laws and regulations)
 
---
 
## Role of SOC in Cybersecurity
The SOC is the operational core of an organization's cybersecurity defense.
It continuously monitors for threats, detects attacks early, and responds before damage spreads.
Without a SOC, threats can go undetected for weeks or months.
 
---
 
## Core Concepts
 
### Threat
Any potential danger that can exploit a weakness to cause harm.
Example: A hacker attempting to steal data.
 
### Vulnerability
A weakness in a system that can be exploited.
Example: Unpatched software, weak passwords.
 
### Risk
Risk = Threat × Vulnerability × Impact
It is the likelihood of a threat exploiting a vulnerability and causing damage.
 
---
 
## CIA Triad
The three foundational principles of cybersecurity:
 
| Principle | Meaning | Example |
|-----------|---------|---------|
| Confidentiality | Only authorized users can access data | Encryption, access controls |
| Integrity | Data is accurate and unmodified | Hashing, digital signatures |
| Availability | Systems and data are accessible when needed | Backups, uptime monitoring |
 
---
 
## Common Cyber Threats
 
### Malware
Malicious software designed to damage or gain unauthorized access.
Types: Virus, Worm, Trojan, Ransomware, Spyware.
 
### Phishing
Attackers trick users into revealing credentials or clicking malicious links
via fake emails or websites.
 
### Insider Threat
A threat that comes from within the organization — a disgruntled employee,
careless staff, or a compromised account.
 
### APT (Advanced Persistent Threat)
A highly skilled, well-funded attacker (often nation-state) who silently
stays inside a network for a long time to steal data or cause damage.
 
---
 
## Common Attack Types
 
### Brute Force
Attacker tries many username/password combinations until one works.
 
### DDoS (Distributed Denial of Service)
Flooding a server with massive traffic from multiple sources to make it unavailable.
 
### Zero-Day
Exploiting a vulnerability that the vendor doesn't know about yet — no patch exists.
 
### SQL Injection
Injecting malicious SQL code into a web form input to manipulate a database.
Example: `' OR '1'='1` bypasses a login form.
 
---
 
## Case Study: WannaCry Ransomware (2017)
- **Type:** Ransomware + Worm
- **Vulnerability Exploited:** EternalBlue (SMB vulnerability in Windows)
- **Impact:** 200,000+ systems infected across 150 countries, hospitals shut down
- **Spread:** Self-propagated through networks without user interaction
- **Lesson:** Patch management and network segmentation are critical
 
---
 
## Cyber Kill Chain
A model describing the stages of a cyberattack (by Lockheed Martin):
 
1. **Reconnaissance** – Attacker gathers information about the target
2. **Weaponization** – Creates malware or exploit
3. **Delivery** – Sends the weapon (phishing email, USB, etc.)
4. **Exploitation** – Executes the exploit on the victim's system
5. **Installation** – Installs malware/backdoor
6. **Command & Control (C2)** – Attacker remotely controls the system
7. **Actions on Objectives** – Steals data, destroys systems, or spreads further
 
> SOC analysts use the Kill Chain to identify at which stage an attack is and stop it early.
 
---
 
## Defense in Depth
A layered security strategy — if one layer fails, others still protect.
 
| Layer | What it Protects | Example Tools/Methods |
|-------|-----------------|----------------------|
| Perimeter | Organization boundary | Firewall, DMZ |
| Network | Internal traffic | IDS/IPS, Segmentation |
| Endpoint | Devices | EDR, Antivirus |
| Application | Software | WAF, Secure coding |
| Data | Files and databases | Encryption, DLP |
| Human Awareness | Users | Security training, phishing simulations |
 
---
 
## Network Security Basics
 
### Key Concepts
- **IP Address** – Unique identifier for a device on a network
- **Port** – Logical channel for communication (e.g., Port 80 = HTTP, Port 443 = HTTPS, Port 22 = SSH)
- **Protocols** – Rules for communication (TCP, UDP, HTTP, DNS, FTP)
 
### Security Devices
- **Firewall** – Filters traffic based on rules (allow/deny)
- **IDS (Intrusion Detection System)** – Detects and alerts on suspicious activity
- **IPS (Intrusion Prevention System)** – Detects AND blocks suspicious activity
- **Network Segmentation** – Divides a network into zones to limit attacker movement
 
---
 
## What is a SIEM?
**SIEM = Security Information and Event Management**
 
A SIEM collects logs from all sources, correlates events, and generates alerts.
It is the central tool used by SOC analysts.
 
Key Functions:
- Log collection and aggregation
- Real-time alerting
- Correlation of events across systems
- Dashboards for monitoring
 
Examples: **Splunk, IBM QRadar, Microsoft Sentinel**
 
---
 
## Common Log Sources
 
| Log Source | What it Tells Us |
|------------|-----------------|
| Windows Event Logs | Login attempts, process execution, user activity |
| Firewall Logs | Allowed/blocked traffic, source/destination IPs |
| VPN Logs | Remote access sessions, unusual login locations |
| DNS Logs | Which domains were queried — useful for detecting C2 traffic |
 
---
 
## Why This Matters for Me
- CIA Triad is the foundation behind every security decision
- Kill Chain helps me understand attacker steps so I can detect them at each stage
- SIEM is my primary tool as an L1 analyst
- Log analysis is the daily work — knowing what each log source tells me is essential
 