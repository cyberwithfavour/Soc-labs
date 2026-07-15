# Alert Investigation Report

## Investigation ID

SOC-003

---

## Alert Summary

**Alert Name:** Unauthorized Administrator Account Creation

**Alert Source:** SIEM

**Category:** Privilege Escalation / Account Management

**Date:** (Today's Date)

---

## Alert Description

The SIEM detected the creation of a new local administrator account at **2:17 AM**, outside normal business hours.

This activity is suspicious because administrator accounts should only be created by authorized personnel during approved maintenance periods.

---

## Initial Assessment

The alert is considered suspicious because:

- The activity occurred outside business hours.
- A privileged account was created.
- No approved maintenance activity was scheduled.
- Unauthorized administrator accounts are commonly created after a system compromise.

---

## Relevant Windows Event IDs

- **4720** – User Account Created
- **4728** – User Added to Security Group
- **4672** – Special Privileges Assigned to New Logon
- **4624** – Successful Logon
- **4625** – Failed Logon Attempts (if applicable)

---

## Severity

**High**

---

## Analyst Actions

- Reviewed the SIEM alert.
- Identified the newly created administrator account.
- Checked authentication logs.
- Verified whether the account creation was authorized.
- Reviewed recent administrator activities.
- Escalated the alert to Tier 2.

---

## Recommendations

- Verify the legitimacy of the account with the IT administrator.
- Disable the account if unauthorized.
- Reset affected administrator credentials if compromise is suspected.
- Review all recent administrative changes.
- Continue monitoring for additional suspicious activity.

---

## Investigation Status

Escalated to Tier 2 Analyst
