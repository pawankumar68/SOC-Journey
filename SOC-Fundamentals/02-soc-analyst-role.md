# SOC Analyst Roles and Responsibilities

## SOC Roles

A Security Operations Center (SOC) has different roles to monitor and respond to security incidents.

### L1 Analyst (Tier 1)
- First line of defense
- Monitors alerts from SIEM tools
- Performs initial investigation
- Identifies false positives
- Escalates real threats to L2 analysts

### L2 Analyst (Tier 2)
- Performs deeper investigation
- Analyzes complex incidents
- Conducts threat hunting
- Responds to confirmed attacks

### L3 Analyst
- Expert level analysts
- Conduct malware analysis
- Develop detection rules
- Improve SOC security processes

---

# Core Responsibilities of an L1 Analyst

- Monitor alerts from SIEM
- Investigate suspicious activities
- Validate alerts
- Create and manage incident tickets
- Escalate incidents to higher level analysts

---

# Tools Used by L1 Analysts

## SIEM Tools
Used to monitor and analyze security logs.

Examples:
- Splunk
- IBM QRadar
- Microsoft Sentinel

## Threat Intelligence Tools

Used to check if IPs, domains, or files are malicious.

Examples:
- VirusTotal
- AbuseIPDB
- AlienVault OTX

## Ticketing Systems

Used to track and manage incidents.

Examples:
- ServiceNow
- Jira

---

# Basic Investigation Process

1. Alert is generated in SIEM.
2. Analyst reviews alert details.
3. Investigates indicators like IP, domain, or file hash.
4. Checks threat intelligence platforms.
5. Determines if the alert is true or false.
6. Escalates confirmed threats to L2 analysts.

---

# Example Investigation

Alert: Suspicious IP connection detected.

Steps:
1. Copy the IP address.
2. Check it on VirusTotal.
3. If flagged malicious by many vendors, it may indicate a threat.
4. Check internal logs for related activity.
5. Create a ticket and escalate if necessary.
