# Timeline

## Investigation ID

005

---

| Time | Event |
|------|-------|
| T0 | Network Intrusion Detection System (NIDS) generated a **Potential Port Scan** alert. |
| T1 | Alert assigned to Tier 1 SOC Analyst for validation. |
| T2 | Source IP identified as **192.168.10.25**. |
| T3 | Alert details reviewed to determine the scope of the activity. |
| T4 | Multiple TCP SYN packets observed targeting several ports on the internal server. |
| T5 | Targeted ports identified: 21, 22, 23, 80, 135, 139, 445, and 3389. |
| T6 | Pattern of activity assessed as consistent with **TCP SYN Port Scanning (Reconnaissance)**. |
| T7 | No evidence of successful exploitation, authentication, or privilege escalation found during the initial investigation. |
| T8 | Alert severity assessed as **Medium**. |
| T9 | Findings documented and recommendations prepared. |
| T10 | Investigation escalated to Tier 2 SOC for continued monitoring and further analysis if additional suspicious activity is observed. |

---

# Investigation Summary

The investigation identified activity consistent with a reconnaissance attempt through TCP SYN port scanning.

No indicators of successful compromise were observed during the initial review. The incident was documented and escalated for continued monitoring and further investigation if necessary.
