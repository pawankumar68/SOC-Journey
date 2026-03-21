# Day 3 – Assignments
 
---
 
## Assignment 1 – Malicious URL Analysis (VirusTotal)
**Tool:** https://www.virustotal.com
 
### Steps Performed
1. Went to VirusTotal → URL tab
2. Pasted the suspicious URL and hit Enter
3. Reviewed the Detection tab — vendor analysis and crowdsourced context
4. Reviewed the Details tab — categories, history, and HTTP response info
 
### Findings
 
| Field | Result |
|-------|--------|
| URL Analyzed | http://194.165.16.11/bin/mirai.arm |
| Hosting IP | 194.165.16.11 |
| Detection Score | **12 / 95** security vendors flagged as malicious |
| Categories Flagged | Malicious (alphaMountain.ai), Spyware and Malware (Sophos), Phishing and Other Frauds (Webroot) |
| Vendors That Flagged | ADMINUSLabs — Malicious, BitDefender — Phishing, Sophos — Spyware and Malware, Webroot — Phishing and Other Frauds, alphaMountain.ai — Malicious |
| Crowdsourced Intel | **MEDIUM** alert — Honeytrap (ArcSight Threat Intelligence): IP domains may infect visitors with malware |
| Behavior (CrowdSec) | SMB/RDP Bruteforce, SSH Bruteforce |
| First Submission | 2026-03-21 17:03:57 UTC |
| Last Analysis | 2026-03-21 17:03:57 UTC |
 
### Screenshots
![VirusTotal Details Tab](images/01-virustotal-details.png)
![VirusTotal Detection Tab](images/02-virustotal-detection.png)
 
### Verdict
**MALICIOUS** — Confirmed malicious by 12 out of 95 security vendors.
 
The filename `mirai.arm` is associated with the **Mirai botnet** — malware that
targets IoT devices (routers, cameras) and enslaves them into a botnet for DDoS attacks.
The `.arm` extension indicates this is a compiled binary for ARM architecture devices.
 
The IP is also actively performing SSH and SMB/RDP bruteforce attacks,
meaning it is being used as attack infrastructure — not just hosting malware.