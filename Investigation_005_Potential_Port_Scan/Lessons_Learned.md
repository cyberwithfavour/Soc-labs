# Lessons Learned

## Investigation ID

005

---

# Overview

This investigation focused on analyzing an IDS alert that identified a potential TCP SYN port scan against an internal server.

The objective was to validate the alert, determine the nature of the activity, assess its severity, and recommend appropriate next steps.

---

# Key Lessons

### 1. Not Every Alert Means a Compromise

An IDS alert indicates suspicious activity, but it does not automatically mean a system has been compromised. Every alert must be validated before conclusions are made.

---

### 2. Port Scanning is Often the First Stage of an Attack

Port scanning is a reconnaissance technique used by attackers to identify open ports and services before attempting exploitation.

Recognizing this behavior early allows security teams to respond before an attack progresses.

---

### 3. Context Matters

The same activity can be either legitimate or malicious.

For example, an authorized vulnerability scanner may perform port scans as part of routine security assessments.

Analysts should always verify whether suspicious activity originates from an approved source.

---

### 4. Documentation is Essential

A well-documented investigation ensures that other analysts can understand the findings, continue the investigation if necessary, and maintain an accurate incident record.

---

### 5. Escalation Should Be Evidence-Based

Since no evidence of successful exploitation was observed, the alert was classified as **Medium** severity and escalated for continued monitoring rather than immediate containment.

---

# Skills Strengthened

- IDS Alert Analysis
- Reconnaissance Detection
- Port Scan Identification
- Threat Assessment
- Incident Documentation
- SOC Investigation Workflow
- Security Analysis

---

# Areas for Improvement

In future investigations, I would like to:

- Analyze packet captures using Wireshark to confirm the scanning technique.
- Correlate IDS alerts with firewall and SIEM logs.
- Identify the scanning tool used (e.g., Nmap).
- Practice distinguishing authorized vulnerability scans from malicious reconnaissance.

---

# Reflection

This investigation helped me understand how SOC analysts approach IDS alerts. Rather than assuming an attack has occurred, the focus is on validating the alert, gathering evidence, assessing the risk, and documenting findings before making informed decisions.

Each investigation strengthens my analytical thinking and prepares me for real-world SOC operations.
