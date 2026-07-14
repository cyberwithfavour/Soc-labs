# Alert Investigation Report

## Investigation ID

SOC-002

---

## Alert Summary

**Alert Name:** Suspicious PowerShell Execution

**Alert Source:** SIEM

**Category:** Endpoint Activity

**Date:** (Today's Date)

---

## Alert Description

The SIEM detected a PowerShell process executing a Base64-encoded command on a company workstation.

Base64 encoding is commonly used by attackers to hide malicious commands and bypass basic detection mechanisms.

---

## Initial Assessment

The alert is suspicious because:

- PowerShell was used to execute an encoded command.
- Encoded commands are often associated with malware or post-exploitation activities.
- Further investigation is required to determine whether the activity was legitimate or malicious.

---

## Severity

**High**

---

## Analyst Actions

- Reviewed the SIEM alert.
- Identified the affected workstation.
- Checked the user account associated with the activity.
- Recommended reviewing PowerShell logs.
- Recommended checking endpoint protection logs.
- Escalated the alert to Tier 2 for deeper investigation.

---

## Recommendations

- Verify whether the PowerShell command was authorized.
- Review Windows Event Logs and PowerShell Operational Logs.
- Scan the endpoint for malware.
- Isolate the device if malicious activity is confirmed.
- Continue monitoring for additional suspicious behavior.

---

## Investigation Status

Escalated to Tier 2 Analyst
