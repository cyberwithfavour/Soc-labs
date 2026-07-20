# Alert Investigation Report

## Investigation ID

008

---

# Alert Information

**Alert Name**

Rogue Access Point Detected

**Alert Source**

Wireless Intrusion Detection System (WIDS)

**Severity**

High

**Alert Category**

Unauthorized Wireless Device

**Status**

Under Investigation

---

# Incident Summary

The organization's Wireless Intrusion Detection System (WIDS) detected an unauthorized wireless access point broadcasting an SSID similar to the company's legitimate wireless network.

The rogue access point was discovered operating within range of the corporate office, creating a potential risk of users connecting to an unauthorized network and exposing sensitive information.

The alert requires immediate investigation to determine whether the device is malicious or an unauthorized personal access point.

---

# Initial Findings

- An unknown wireless access point was detected.
- The SSID closely resembled the organization's official Wi-Fi network.
- The device was not listed in the organization's authorized wireless inventory.
- Several wireless clients attempted to associate with the rogue access point.
- The device was broadcasting on the same wireless channel as the corporate network.

---

# Indicators of Compromise (IOCs)

- Unknown wireless access point detected.
- Similar SSID to the corporate wireless network.
- Unauthorized MAC address.
- Unknown device manufacturer.
- Unexpected wireless clients attempting to connect.

---

# Risk Assessment

A rogue access point introduces significant security risks because it can be used to:

- Capture user credentials.
- Intercept sensitive network traffic.
- Launch Man-in-the-Middle (MitM) attacks.
- Provide attackers with unauthorized network access.
- Bypass existing network security controls.

If confirmed as malicious, the incident could result in credential theft or compromise of corporate systems.

---

# Analyst Assessment

Based on the available evidence, the wireless device is considered **unauthorized** and presents a **High** security risk.

Further investigation is required to determine whether the device is an employee-installed access point or part of an Evil Twin attack.

---

# Recommended Actions

- Locate the physical device.
- Disconnect the rogue access point from the network.
- Block the device's MAC address.
- Verify whether any users connected to the rogue network.
- Reset passwords for affected users if credential theft is suspected.
- Continue monitoring for additional unauthorized wireless devices.
- Escalate the incident if malicious activity is confirmed.
