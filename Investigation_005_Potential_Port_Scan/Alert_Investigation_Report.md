# Alert Investigation Report

## Investigation Details

**Investigation ID:** 005

**Date:** Day 50 of Cybersecurity Journey

**Analyst:** Favour

**Alert Source:** Network Intrusion Detection System (NIDS)

**Alert Name:** Potential Port Scan

**Priority:** Medium

**Status:** Escalated

---

# Alert Summary

The Network Intrusion Detection System generated an alert after detecting multiple TCP SYN packets from a single internal host attempting to connect to several ports on an internal server within 30 seconds.

The activity is consistent with reconnaissance behavior commonly observed during the early stages of a cyber attack.

---

# Alert Details

**Source IP Address**

192.168.10.25

**Destination**

Internal Server

**Ports Targeted**

- 21 (FTP)
- 22 (SSH)
- 23 (Telnet)
- 80 (HTTP)
- 135 (RPC)
- 139 (NetBIOS)
- 445 (SMB)
- 3389 (RDP)

---

# Initial Analysis

The source host attempted connections to multiple ports within a short period.

This behavior matches the characteristics of a **TCP SYN Port Scan**, where an attacker attempts to identify open services before launching additional attacks.

No successful exploitation attempts were identified during the initial review.

---

# Findings

- IDS alert successfully validated.
- Multiple connection attempts observed.
- Reconnaissance activity suspected.
- No evidence of privilege escalation.
- No evidence of malware execution.
- No evidence of successful compromise.

---

# Risk Assessment

**Severity:** Medium

**Reason**

Although no systems appear to have been compromised, reconnaissance activity is considered suspicious because attackers often perform port scans to identify vulnerable services before exploitation.

---

# Recommended Actions

- Review firewall logs for additional activity.
- Verify whether the source IP belongs to an authorized vulnerability scanner.
- Continue monitoring the source host.
- Block the source IP if malicious activity continues.
- Escalate to Tier 2 SOC for deeper investigation if required.

---

# Investigation Outcome

The alert was determined to be a **suspected TCP SYN Port Scan**.

At this stage, there is insufficient evidence to confirm compromise. Continued monitoring and additional log analysis are recommended.
