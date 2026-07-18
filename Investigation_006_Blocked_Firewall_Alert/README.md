# Investigation 006 – Blocked Firewall Alert

## Scenario

The organization's firewall generated an alert after blocking an outbound HTTPS connection from an internal workstation to an IP address listed in the organization's threat intelligence feed as malicious.

The alert was automatically forwarded to the SIEM for investigation.

---

## Objective

Investigate the firewall alert, determine why the connection was blocked, assess the potential risk to the organization, and recommend appropriate next steps.

---

## Investigation Summary

- Alert Source: Firewall
- Alert Type: Blocked Outbound Connection
- Source Host: 192.168.15.35
- Destination IP: 185.231.54.20
- Destination Port: TCP 443 (HTTPS)
- Severity: High
- Status: Escalated

---

## Skills Demonstrated

- Firewall Alert Analysis
- Threat Intelligence Validation
- Outbound Traffic Investigation
- Threat Assessment
- Incident Documentation
- SOC Investigation Workflow

---

## Tools

- Firewall
- SIEM
- Threat Intelligence Feed
- Endpoint Security Logs
- Network Logs

---

## Outcome

The firewall successfully blocked communication between an internal workstation and a known malicious IP address.

Although the connection was prevented, the activity indicates possible malware infection or suspicious behavior on the endpoint. Further investigation is required to determine the root cause.
