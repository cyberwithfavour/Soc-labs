# Evidence

## Investigation ID

006

---

# Alert Information

**Alert Source**

Firewall

**Alert Type**

Blocked Outbound Connection

**Severity**

High

**Firewall Action**

Blocked

---

# Source Information

**Source Host**

192.168.15.35

---

# Destination Information

**Destination IP**

185.231.54.20

**Destination Port**

TCP 443 (HTTPS)

---

# Threat Intelligence

The destination IP address matched an entry in the organization's Threat Intelligence Feed and is classified as a **known malicious IP**.

---

# Indicators Observed

- Outbound HTTPS connection attempt detected.
- Firewall successfully blocked the connection.
- Destination IP identified as malicious.
- Communication attempt originated from an internal workstation.
- No successful connection established.
- Potential Command-and-Control (C2) communication suspected.

---

# Evidence Collected

- Firewall Alert
- Source Host IP Address
- Destination Malicious IP
- Destination Port (443)
- Firewall Action (Blocked)
- Threat Intelligence Match
- Initial Traffic Analysis

---

# Assessment

The firewall successfully prevented communication with a known malicious IP address.

Although no connection was established, the attempted communication suggests the endpoint may be compromised or running malicious software.

Additional endpoint analysis is required to determine the root cause.

---

# Recommendation

- Perform a full malware scan on the endpoint.
- Review SIEM logs for related alerts.
- Check DNS and proxy logs for previous connections.
- Monitor the workstation for additional suspicious activity.
- Escalate to Tier 2 SOC for further investigation.
