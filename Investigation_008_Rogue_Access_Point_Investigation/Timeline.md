# Timeline

## Investigation ID

008

---

| Time | Event |
|------|-------|
| 10:12 AM | Wireless Intrusion Detection System (WIDS) detected a new wireless access point broadcasting the SSID **Corporate_WiFi_Free**. |
| 10:13 AM | WIDS classified the access point as **Unauthorized** because it was not found in the organization's wireless asset inventory. |
| 10:14 AM | Three employee devices attempted to connect to the rogue access point. |
| 10:15 AM | SIEM generated a **High Severity Rogue Access Point Alert**. |
| 10:17 AM | Tier 1 SOC analyst received the alert and initiated investigation. |
| 10:20 AM | SSID, MAC address, and wireless channel were compared against the organization's authorized access points. |
| 10:24 AM | Investigation confirmed the device was broadcasting a network name similar to the legitimate corporate Wi-Fi. |
| 10:27 AM | Risk assessment determined the possibility of an **Evil Twin Attack** targeting employee credentials. |
| 10:30 AM | Recommendation made to locate and isolate the rogue access point immediately. |
| 10:35 AM | Incident escalated to the Network Security Team for physical identification and removal of the unauthorized device. |

---

# Investigation Summary

The investigation identified an **unauthorized wireless access point** operating within the organization's premises.

The device was broadcasting an SSID that closely resembled the legitimate corporate wireless network, increasing the likelihood that employees could unknowingly connect to it.

Because multiple connection attempts were observed and the access point was not part of the organization's approved infrastructure, the incident was classified as **High Severity** and escalated for immediate containment and further investigation.
