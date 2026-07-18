# Investigation 005 – Potential Port Scan

## Scenario

The Network Intrusion Detection System (NIDS) generated an alert after detecting multiple TCP SYN packets originating from a single internal host targeting several ports on an internal server within a short period.

The activity was classified as a **Potential Port Scan**.

---

## Objective

Investigate the IDS alert, identify the source of the activity, determine whether it is malicious or authorized, assess the severity, and recommend the appropriate response.

---

## Investigation Summary

- Alert Source: Network IDS
- Alert Type: Potential Port Scan
- Source IP: 192.168.10.25
- Destination: Internal Server
- Severity: Medium
- Status: Escalated for further investigation

---

## Skills Demonstrated

- IDS Alert Analysis
- Network Monitoring
- Port Scan Identification
- Alert Validation
- Incident Documentation
- Threat Assessment
- SOC Investigation Workflow

---

## Tools

- IDS
- SIEM
- Network Logs
- Firewall Logs

---

## Outcome

The investigation identified behavior consistent with reconnaissance activity.

Although no exploitation attempts were observed, additional monitoring and investigation were recommended because reconnaissance is often the first stage of a cyber attack.
