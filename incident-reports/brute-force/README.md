# 🚨 Brute Force Attack Investigation

## 📌 Overview

This investigation focuses on identifying and analyzing repeated failed authentication attempts that may indicate a brute-force attack.

The objective is to determine whether the observed activity is malicious, identify the affected account and source, and recommend appropriate response actions.

---

## 🎯 Investigation Objectives

- Identify repeated failed authentication attempts
- Identify the source IP address
- Identify the targeted account
- Determine whether a successful login occurred
- Analyze the timeline of events
- Identify potential Indicators of Compromise (IOCs)
- Map the activity to MITRE ATT&CK
- Determine the severity
- Recommend appropriate response actions

---

## 🛠️ Tools Used

- SIEM
- Windows Event Viewer / Linux Authentication Logs
- VirusTotal
- Wireshark
- MITRE ATT&CK

---

## 🔔 Alert Information

| Field | Details |
|---|---|
| Alert Type | Multiple Failed Logins |
| Attack Type | Suspected Brute Force |
| Source IP | `LAB-IP` |
| Target Account | `LAB-ACCOUNT` |
| Target Host | `LAB-HOST` |
| Protocol | SSH / RDP / Authentication |
| Severity | Medium |
| Status | Investigating |

---

## 🔎 Investigation

### Step 1 — Analyze Authentication Attempts

The authentication logs were reviewed to identify repeated failed login attempts.

Example:

```text
Failed authentication attempt
Failed authentication attempt
Failed authentication attempt
Failed authentication attempt
A high number of failed authentication attempts within a short period can indicate possible brute-force activity.

Step 2 — Identify Source IP

The source IP responsible for the authentication attempts was identified.

Source IP: LAB-IP

The IP should be investigated using appropriate threat intelligence sources.

Step 3 — Identify Target Account

The targeted account was identified from the authentication logs.

Target Account: LAB-ACCOUNT

The account should be checked to determine whether it is a privileged or standard user account.

Step 4 — Check for Successful Authentication

After identifying repeated failed attempts, successful authentication events should be reviewed.

Example:

Failed Login
Failed Login
Failed Login
Failed Login
Successful Login

A successful login following multiple failed attempts requires additional investigation because it may indicate that the attacker obtained valid credentials.

🧩 Indicators of Compromise
IOC Type	Value
Source IP	LAB-IP
Username	LAB-ACCOUNT
Host	LAB-HOST
Timestamp	LAB-TIMESTAMP

All indicators in this report should come from an authorized lab or training environment.

🧠 MITRE ATT&CK Mapping
T1110 — Brute Force

The observed behavior is consistent with repeated authentication attempts against an account.

Possible sub-techniques may include:

T1110.001 — Password Guessing
T1110.002 — Password Cracking
T1110.003 — Password Spraying
T1110.004 — Credential Stuffing

The exact technique/sub-technique should be selected based on the evidence observed during the investigation.

⚠️ Severity Assessment
Severity: Medium

The activity is considered potentially suspicious because multiple authentication failures were observed.

Severity may be increased if:

A successful login occurred
A privileged account was targeted
Suspicious commands were executed
Malware was detected
Lateral movement was observed
Additional IOCs were identified
🚑 Recommended Response
Investigate the source IP.
Check whether authentication was successful.
Review the affected account.
Review activity after successful authentication.
Check for additional suspicious events.
Reset credentials if compromise is suspected.
Enable MFA where possible.
Block or restrict the source where appropriate.
Continue monitoring the affected host and account.
Escalate the incident if compromise is confirmed.
📝 Conclusion

The investigation identified repeated authentication failures that may indicate a brute-force attack.

Additional correlation with successful authentication events, endpoint activity, source IP reputation, and other security logs is required to determine whether unauthorized access occurred.

📚 Lessons Learned

This investigation demonstrates the importance of:

Authentication log monitoring
Alert triage
Source IP investigation
Account monitoring
Event correlation
IOC analysis
MITRE ATT&CK mapping
Incident documentation
⚠️ Disclaimer

This investigation is intended for cybersecurity education and portfolio purposes.

All testing and analysis should be performed only in authorized lab environments, training platforms, or systems for which permission has been granted.
