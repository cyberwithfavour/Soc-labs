# Evidence Collected

## Alert Information

- SIEM alert for excessive DNS requests.
- More than 500 DNS queries generated within 10 minutes.

---

## Network Information

- Protocol: DNS
- Port: 53
- Destination: Unknown Domain

---

## Systems Involved

- Employee Workstation
- Internal DNS Server

---

## Evidence Reviewed

- DNS Logs
- Firewall Logs
- Network Traffic Logs
- Endpoint Security Logs
- SIEM Correlation Data

---

## Additional Information Required

- Reputation of the destination domain.
- Whether other hosts contacted the same domain.
- Endpoint malware scan results.
- User activity during the alert timeframe.

---

## Initial Finding

The DNS activity appears abnormal and requires further investigation to determine whether it is malicious or a legitimate application generating excessive requests.
