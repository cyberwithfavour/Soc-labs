# Timeline

## Investigation ID

006

---

| Time | Event |
|------|-------|
| T0 | Firewall detected an outbound HTTPS connection attempt from an internal workstation. |
| T1 | Firewall compared the destination IP against the organization's Threat Intelligence Feed. |
| T2 | Destination IP **185.231.54.20** was identified as a known malicious IP address. |
| T3 | Firewall automatically blocked the outbound connection. |
| T4 | Firewall generated a **Blocked Outbound Connection** alert. |
| T5 | Alert was forwarded to the SIEM for analysis. |
| T6 | Tier 1 SOC Analyst received and validated the alert. |
| T7 | Source workstation identified as **192.168.15.35**. |
| T8 | Initial analysis indicated a possible attempt to communicate with a Command-and-Control (C2) server. |
| T9 | Severity assessed as **High** due to the malicious reputation of the destination IP. |
| T10 | Recommendations documented, including endpoint malware scan, log correlation, and continued monitoring. |
| T11 | Investigation escalated to Tier 2 SOC for further endpoint analysis. |

---

# Investigation Summary

The firewall successfully blocked an outbound HTTPS connection from an internal workstation to a known malicious IP address before communication could be established.

Although the connection was prevented, the attempted communication suggests possible endpoint compromise or malware activity. The incident was documented and escalated for further investigation.
