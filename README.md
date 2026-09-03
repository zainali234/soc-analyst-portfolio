# 🛡️ SOC Analyst Portfolio

Welcome to my cybersecurity portfolio.

This repository documents my hands-on learning and practical investigations related to **Security Operations Center (SOC)**, including security monitoring, alert triage, SIEM, network analysis, threat intelligence, phishing analysis, and incident response.

---

## 🎯 Objective

The purpose of this portfolio is to document practical cybersecurity investigations and demonstrate my ability to:

- Analyze security alerts
- Investigate suspicious activity
- Analyze logs
- Identify Indicators of Compromise (IOCs)
- Perform network traffic analysis
- Investigate phishing attempts
- Use SIEM tools
- Map activities to MITRE ATT&CK
- Assess incident severity
- Document findings
- Recommend appropriate response actions

---

# 🔎 Areas of Focus

### 📊 SIEM & Log Analysis
- Splunk
- Elastic / Kibana
- Windows Event Logs
- Linux Logs
- Authentication Events
- Security Event Analysis

### 🌐 Network Security
- TCP/IP
- DNS
- HTTP/HTTPS
- Network Traffic Analysis
- Packet Analysis
- Wireshark
- Nmap

### 🪟 Windows Security
- Windows Event Viewer
- Security Events
- Authentication Monitoring
- PowerShell
- Process Analysis
- Sysmon

### 🐧 Linux Security
- Linux Authentication Logs
- SSH Monitoring
- Process Analysis
- Linux Command Line
- Log Analysis

### 🎣 Threat Intelligence
- IP Investigation
- Domain Investigation
- URL Analysis
- Hash Analysis
- IOC Investigation
- VirusTotal
- CyberChef

### 🧠 Security Frameworks
- MITRE ATT&CK
- Cyber Kill Chain
- Incident Response Lifecycle

---

# 🚨 Investigations

## 🔐 Brute Force Attack Investigation

Investigation of repeated authentication failures to identify potential brute-force activity.

**Investigation areas:**

- Failed login attempts
- Source IP analysis
- Target account analysis
- Successful login correlation
- IOC investigation
- MITRE ATT&CK mapping
- Severity assessment

**MITRE ATT&CK:** T1110 - Brute Force

---

## 🎣 Phishing Email Investigation

Investigation of a suspicious email to identify potential phishing indicators.

**Investigation areas:**

- Email headers
- Sender information
- URLs
- Domains
- Attachments
- File hashes
- Threat intelligence
- Final verdict

---

## 🌐 Network Traffic Investigation

Analysis of network traffic using Wireshark to identify suspicious communication.

**Investigation areas:**

- DNS traffic
- HTTP/HTTPS traffic
- TCP connections
- Source and destination IPs
- Suspicious domains
- Packet analysis

---

## 📊 Splunk Security Investigation

Hands-on SIEM investigation using Splunk to analyze security events and identify suspicious activity.

**Investigation areas:**

- Authentication events
- Failed logins
- Successful logins
- Source IP analysis
- User activity
- Event correlation
- Alert investigation

---

# 🧠 MITRE ATT&CK

MITRE ATT&CK is used to map observed attacker behavior to relevant tactics and techniques.

### Tactics

- Initial Access
- Execution
- Persistence
- Privilege Escalation
- Defense Evasion
- Credential Access
- Discovery
- Lateral Movement
- Collection
- Command and Control
- Exfiltration
- Impact

---

# 🧪 Investigation Methodology

I follow a structured approach when investigating security alerts:

```text
Alert
  ↓
Understand the Event
  ↓
Validate the Alert
  ↓
Collect Evidence
  ↓
Investigate User / Host / IP
  ↓
Identify IOCs
  ↓
Map to MITRE ATT&CK
  ↓
Determine Severity
  ↓
False Positive or True Positive
  ↓
Document Findings
Repository Structure
soc-analyst-portfolio/
│
├── README.md
│
├── incident-reports/
│   ├── brute-force/
│   ├── phishing/
│   ├── suspicious-login/
│   └── malware/
│
├── splunk/
│   ├── queries.md
│   └── investigations/
│
├── wireshark/
│   └── investigations/
│
├── threat-intelligence/
│   ├── ip-analysis.md
│   ├── domain-analysis.md
│   └── hash-analysis.md
│
├── mitre-attack/
│   └── attack-mapping.md
│
└── notes/
    ├── windows-events.md
    ├── linux-logs.md
    └── networking.md
Learning Platform
Learning Platforms

I use hands-on cybersecurity labs and practical exercises to develop my SOC Analyst skills.

Currently focusing on:

SOC Analyst Level 1
SIEM
Splunk
Network Security Monitoring
Windows Security Monitoring
Linux Security Monitoring
Phishing Analysis
Threat Intelligence
Incident Response
MITRE ATT&CK

  ↓
Close or Escalate
