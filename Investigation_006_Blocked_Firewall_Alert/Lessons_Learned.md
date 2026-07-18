# Lessons Learned

## Investigation ID

006

---

# Overview

This investigation focused on analyzing a firewall alert that blocked an outbound HTTPS connection from an internal workstation to a known malicious IP address.

The objective was to validate the alert, assess the potential risk, determine the appropriate response, and document the investigation following the SOC workflow.

---

# Key Lessons

### 1. A Blocked Connection Does Not Mean the Investigation Ends

Although the firewall successfully blocked the outbound connection, the alert still required investigation.

A blocked connection may indicate that an internal device attempted to communicate with a malicious server, which could be a sign of malware infection or endpoint compromise.

---

### 2. Threat Intelligence Adds Valuable Context

The firewall identified the destination IP using the organization's Threat Intelligence Feed.

Threat intelligence helps analysts quickly determine whether an IP address, domain, or file hash has a known malicious reputation, allowing faster decision-making during investigations.

---

### 3. Outbound Traffic Can Be Just as Important as Inbound Traffic

Cybersecurity is not only about preventing attackers from entering a network.

Monitoring outbound traffic is equally important because compromised systems often attempt to communicate with external Command-and-Control (C2) servers, download additional malware, or exfiltrate sensitive data.

---

### 4. Firewall Logs Are an Important Source of Evidence

Firewall logs provide valuable information such as:

- Source IP address
- Destination IP address
- Ports
- Protocols
- Firewall action (Allowed or Blocked)

These logs help analysts understand what happened and support incident investigations.

---

### 5. Correlation Improves Investigations

A firewall alert alone does not provide the complete picture.

SOC analysts should correlate firewall logs with:

- SIEM alerts
- Endpoint Detection and Response (EDR) logs
- DNS logs
- Proxy logs
- Endpoint antivirus alerts

This helps determine whether the activity is isolated or part of a larger attack.

---

# Skills Strengthened

- Firewall Alert Analysis
- Threat Intelligence Validation
- Malicious IP Investigation
- Outbound Traffic Analysis
- Incident Documentation
- Risk Assessment
- SOC Investigation Workflow

---

# Areas for Improvement

In future investigations, I would like to:

- Correlate firewall alerts with Microsoft Sentinel investigations.
- Investigate DNS queries related to malicious domains.
- Analyze packet captures using Wireshark.
- Learn how EDR solutions validate endpoint compromise.
- Practice identifying Command-and-Control (C2) traffic.

---

# Reflection

This investigation helped me understand that a firewall is not only a preventive security control but also an important source of evidence during incident response.

Even when malicious traffic is blocked, analysts must still determine **why** the communication was attempted and whether the endpoint requires further investigation.

Every SOC investigation improves my ability to think critically, analyze security events, and document findings in a structured and professional manner.
