# Alert Investigation Report

## Investigation ID

SOC-004

---

## Alert Summary

**Alert Name:** Suspicious DNS Traffic

**Alert Source:** SIEM

**Category:** Network Activity

**Date:** (July 16th 2026)

---

## Alert Description

The SIEM detected that a workstation generated more than **500 DNS requests** to an unknown domain within a 10-minute period.

Excessive DNS requests are unusual and may indicate malware attempting to communicate with a command-and-control (C2) server or using DNS tunneling to transfer data.

---

## Initial Assessment

The alert is considered suspicious because:

- A large number of DNS requests were generated in a short period.
- The destination domain is unknown.
- Normal user activity typically does not generate this volume of DNS queries.
- DNS is commonly abused by attackers for persistence and covert communication.

---

## Relevant Network Information

**Protocol:** DNS

**Port:** 53

**Affected Asset:** Employee Workstation

---

## Severity

**High**

---

## Analyst Actions

- Reviewed the SIEM alert.
- Confirmed the volume of DNS requests.
- Identified the affected workstation.
- Checked the reputation of the destination domain.
- Reviewed recent network activity from the host.
- Escalated the incident to Tier 2 for deeper analysis.

---

## Recommendations

- Isolate the affected workstation if malicious activity is confirmed.
- Block communication with the suspicious domain.
- Perform a malware scan on the endpoint.
- Review DNS logs for similar activity on other systems.
- Continue monitoring network traffic for additional indicators of compromise.

---

## Investigation Status

Escalated to Tier 2 Analyst.
