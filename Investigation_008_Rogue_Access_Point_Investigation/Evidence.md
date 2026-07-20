# Evidence

## Investigation ID

008

---

# Evidence Collected

## Wireless Intrusion Detection Logs

| Time | SSID | BSSID (MAC Address) | Status |
|------|------|----------------------|--------|
| 10:12 AM | Corporate_WiFi | 00:1A:2B:3C:4D:5E | Authorized |
| 10:14 AM | Corporate_WiFi_Free | A4:7B:9C:12:8D:45 | Unauthorized |

---

## Rogue Access Point Details

**SSID:** Corporate_WiFi_Free

**MAC Address:** A4:7B:9C:12:8D:45

**Vendor:** Unknown

**Channel:** 6

**Signal Strength:** Strong

**Location:** Third Floor Office Area

---

## Authorized Access Point

**SSID:** Corporate_WiFi

**MAC Address:** 00:1A:2B:3C:4D:5E

**Vendor:** Cisco

**Channel:** 11

---

## Connected Clients

Three devices attempted to connect to the rogue access point:

| Device | Status |
|---------|--------|
| Laptop-023 | Connection Attempted |
| Mobile-014 | Connection Attempted |
| Laptop-031 | Authentication Failed |

---

## Log Analysis

The rogue access point was broadcasting a network name similar to the organization's legitimate wireless network.

Its strong signal strength increased the likelihood that employees could mistakenly connect to it instead of the legitimate corporate Wi-Fi.

No authorization records were found for the device in the organization's wireless asset inventory.

---

## Indicators of Suspicious Activity

- Unauthorized wireless access point.
- Similar SSID to the corporate network.
- Unknown MAC address.
- Unknown hardware vendor.
- Multiple connection attempts from corporate devices.
- Strong signal within the office environment.

---

# Evidence Summary

The collected evidence confirms the presence of an unauthorized wireless access point operating inside the organization's premises.

Because the rogue device imitated the corporate Wi-Fi name and attracted connection attempts from employee devices, the likelihood of an **Evil Twin** attack is considered high.

Immediate containment and removal of the device are recommended to prevent credential theft and unauthorized access.
