# Alert Investigation Report

## Investigation Details

**Investigation ID:** 006

**Date:** Day 51 of Cybersecurity Journey

**Analyst:** Favour

**Alert Source:** Firewall

**Alert Name:** Blocked Outbound Connection to Known Malicious IP

**Priority:** High

**Status:** Escalated

---

# Alert Summary

The organization's firewall generated an alert after blocking an outbound HTTPS connection from an internal workstation to a destination IP address listed in the organization's threat intelligence feed as malicious.

The firewall successfully prevented communication and forwarded the alert to the SIEM for investigation.

---

# Alert Details

## Source Host

192.168.15.35

## Destination IP

185.231.54.20

## Destination Port

TCP 443 (HTTPS)

## Firewall Action

Blocked

---

# Initial Analysis

The firewall detected an outbound connection attempt from an internal workstation to a known malicious IP address.

Because the destination IP is included in the organization's threat intelligence feed, the activity is considered suspicious and may indicate:

- Malware attempting Command-and-Control (C2) communication.
- A compromised endpoint.
- A user attempting to access a malicious website.
- A potentially unwanted application initiating the connection.

The firewall successfully blocked the communication before a connection could be established.

---

# Findings

- Firewall alert successfully validated.
- Outbound HTTPS connection blocked.
- Destination IP identified as malicious.
- No successful communication established.
- Potential malware infection cannot be ruled out.
- Additional endpoint investigation required.

---

# Risk Assessment

**Severity:** High

### Reason

Although the firewall blocked the traffic, an internal workstation attempted to communicate with a known malicious IP address.

This behavior may indicate an infected or compromised endpoint requiring immediate investigation.

---

# Recommended Actions

- Review endpoint security logs.
- Perform a malware scan on the workstation.
- Review SIEM logs for related alerts.
- Review DNS and proxy logs for additional connections.
- Verify whether the connection originated from a legitimate application.
- Continue monitoring the endpoint.
- Escalate the incident to Tier 2 SOC for further analysis.

---

# Investigation Outcome

The firewall successfully prevented communication with a known malicious IP address.

No evidence of successful external communication was observed during the initial investigation.

The incident has been escalated for additional endpoint analysis to determine whether the workstation has been compromised.
