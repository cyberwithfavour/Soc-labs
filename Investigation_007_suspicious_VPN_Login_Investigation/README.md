# SOC Investigation #007

# README

## Investigation Title

Suspicious VPN Login Investigation (Impossible Travel)

---

## Scenario

The Security Operations Center (SOC) received an alert after a user account authenticated successfully through the company's VPN from two geographically distant locations within a short period.

### Login Activity

| Time | Location | Status |
|------|----------|--------|
| 08:15 AM | Lagos, Nigeria | Successful Login |
| 08:40 AM | Toronto, Canada | Successful Login |

Since it is physically impossible for the same user to travel between these locations in 25 minutes, the SIEM generated an **Impossible Travel** alert.

Your task is to investigate whether the activity is legitimate or indicates a compromised account.

---

## Investigation Objectives

- Validate the alert.
- Review VPN authentication logs.
- Identify the source IP addresses.
- Verify user activity.
- Assess the severity of the incident.
- Recommend appropriate response actions.
- Document the investigation following SOC procedures.

---

## MITRE ATT&CK Mapping

| Tactic | Technique |
|---------|-----------|
| Initial Access | Valid Accounts (T1078) |
| Credential Access | Use of Stolen Credentials |
| Defense Evasion | Legitimate VPN Access |

---

## Skills Practiced

- VPN Log Analysis
- Authentication Investigation
- Geolocation Analysis
- Impossible Travel Detection
- Incident Documentation
- Risk Assessment
- SOC Investigation Workflow

---

## Outcome

This investigation demonstrates how SOC analysts identify suspicious VPN authentication activity, determine whether an account may have been compromised, and recommend appropriate containment and response actions.
