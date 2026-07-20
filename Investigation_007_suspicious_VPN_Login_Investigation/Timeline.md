# Timeline

## Investigation ID

007

---

| Time | Event |
|------|-------|
| 08:15 AM | User **j.doe** successfully authenticated to the corporate VPN from **Lagos, Nigeria**. |
| 08:16 AM | VPN gateway established a secure encrypted session for the user. |
| 08:40 AM | The same user account successfully authenticated to the VPN from **Toronto, Canada**. |
| 08:40 AM | SIEM correlated both authentication events and identified an **Impossible Travel** pattern. |
| 08:41 AM | SIEM generated a **High Severity Impossible Travel Alert**. |
| 08:43 AM | Tier 1 SOC analyst received the alert and began initial triage. |
| 08:47 AM | VPN authentication logs and source IP addresses were reviewed. |
| 08:50 AM | Historical login activity showed no previous VPN access from Canada for this user. |
| 08:55 AM | Initial assessment indicated possible credential compromise. |
| 09:00 AM | Recommendation made to verify the user's activity, terminate active VPN sessions if necessary, and reset credentials if compromise is confirmed. |
| 09:05 AM | Incident escalated to Tier 2 SOC for further investigation and endpoint analysis. |

---

# Investigation Summary

The SIEM detected an **Impossible Travel** event after the same VPN account authenticated successfully from **Lagos, Nigeria**, and **Toronto, Canada**, within a **25-minute** period.

The authentication pattern is inconsistent with legitimate user behavior and is commonly associated with stolen credentials or unauthorized account access.

Based on the available evidence, the incident was classified as **High Severity** and escalated for further investigation to determine whether the account had been compromised.
