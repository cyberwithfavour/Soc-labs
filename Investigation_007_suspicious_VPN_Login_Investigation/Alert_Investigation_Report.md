# Alert Investigation Report

## Investigation ID

007

---

# Alert Information

**Alert Name**

Impossible Travel VPN Login

**Alert Source**

Security Information and Event Management (SIEM)

**Severity**

High

**Alert Category**

Suspicious Authentication Activity

**Status**

Under Investigation

---

# Incident Summary

The SIEM generated an **Impossible Travel** alert after detecting two successful VPN logins for the same user account from different countries within a 25-minute window.

The first authentication originated from **Lagos, Nigeria**, while the second originated from **Toronto, Canada**.

The short time difference between both logins makes legitimate travel highly unlikely and may indicate compromised credentials.

---

# Initial Findings

- Two successful VPN authentications were recorded.
- Both logins used the same user account.
- The logins originated from different countries.
- Time difference between both logins was approximately 25 minutes.
- No failed login attempts were observed before the successful authentications.
- The account has never previously logged in from Canada.

---

# Indicators of Compromise (IOCs)

- Successful VPN authentication from multiple geographic locations.
- Impossible travel behavior.
- New source IP address.
- Unusual login location.
- Potential stolen credentials.

---

# Risk Assessment

Because the user successfully authenticated from two geographically distant locations within a very short period, there is a high probability that the account credentials have been compromised.

If confirmed, the attacker may have gained unauthorized access to internal company resources through the VPN.

---

# Analyst Assessment

Based on the available evidence, this activity is considered **highly suspicious**.

Although legitimate explanations such as VPN exit nodes or user travel are possible, the timeline and login pattern strongly suggest potential credential compromise.

Additional verification with the user and endpoint investigation are required before closing the incident.

---

# Recommended Actions

- Contact the user to verify recent login activity.
- Review VPN authentication logs.
- Review MFA logs.
- Check endpoint activity after authentication.
- Search for additional suspicious logins.
- Reset the user's password if compromise is confirmed.
- Terminate active VPN sessions.
- Escalate the incident to Tier 2 SOC for further investigation.
