# Offensive Security Intro

## Room Info
- Path: Pre-Security > Introduction to Cyber Security > Offensive Security Intro
- Status: ✅ Completed

## Task 1 — Think Like a Hacker
Offensive security knowledge is equally important for defenders.
By thinking like an attacker, we can identify bugs and
vulnerabilities before they are exploited — and fix them proactively.
This is the core philosophy of ethical hacking.

## Task 2 — Starting the Lab
Accessed a simulated bank website interface.
Goal was to find a specific account number within the application.
This introduced the concept of web application reconnaissance.

## Task 3 — Find Hidden Pages
Used **Dirb** — a web content scanner tool.

Command used:
```
dirb <target-url>
```
- Dirb scans a website for hidden directories and pages
- Lines starting with **+** = found/existing URLs
- This technique is called directory brute forcing

## Task 4 — Attack the Admin Page
Found a hidden admin panel by adding `/bank-transfer` to the URL.
This revealed a page that allowed unauthorized money transfers.
This demonstrates how hidden but unprotected pages can be
exploited by attackers — a common web application vulnerability.

## Key Tools Learned
| Tool | Purpose |
|------|---------|
| Dirb | Web content scanner — finds hidden pages and directories |

## How This Connects to Real SOC Work
- SOC analysts must understand offensive techniques to detect them
- Directory brute forcing generates unusual traffic — detectable in logs
- Hidden admin panels without authentication = critical vulnerability
- Thinking like an attacker helps defenders protect systems better
