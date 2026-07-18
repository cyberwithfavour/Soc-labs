# Evidence

## Investigation ID

005

---

# Alert Information

**Alert Source**

Network Intrusion Detection System (NIDS)

**Alert Type**

Potential Port Scan

**Severity**

Medium

---

# Source Information

**Source IP Address**

192.168.10.25

---

# Target Information

Internal Server

---

# Targeted Ports

| Port | Service |
|------:|----------|
| 21 | FTP |
| 22 | SSH |
| 23 | Telnet |
| 80 | HTTP |
| 135 | RPC |
| 139 | NetBIOS |
| 445 | SMB |
| 3389 | RDP |

---

# Indicators Observed

- Multiple TCP SYN packets detected.
- Connection attempts to multiple ports within 30 seconds.
- Reconnaissance behavior identified.
- No successful authentication attempts observed.
- No evidence of privilege escalation.
- No malware activity detected during initial review.

---

# Evidence Collected

- IDS Alert
- Source IP Address
- Destination Server
- List of Targeted Ports
- Network Connection Pattern
- Initial Traffic Analysis

---

# Assessment

The observed activity is consistent with a TCP SYN Port Scan used during the reconnaissance phase of a cyber attack.

Although there is no evidence of compromise at this stage, the activity is considered suspicious and requires continued monitoring.

---

# Recommendation

- Continue monitoring the source IP.
- Review firewall and SIEM logs for additional activity.
- Verify whether the activity originated from an authorized vulnerability scanner.
- Escalate if further suspicious behavior is detected.
