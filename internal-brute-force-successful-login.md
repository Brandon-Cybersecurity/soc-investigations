# Incident 001 | PRIORITY: 3
## Access Control - T1110 Internal Brute Force with Successful Login

Hello <Company Name>,

---

## Case Reference
Case URL:  
10.xxx.xxx.xxx

Date/Time:  
05/20/2026 1:45 AM CDT

---

## Event Details

Host (Origin):  
HARCOMP001

Host (Impacted):  
ARDVOMP775

User (Origin):  
Josh

Common Events:
- User Logon Failure
- User Logon

Log Source:
- CompanyHAKK

---

## Summary

Multiple failed authentication attempts were observed from the same internal origin host to the same impacted host, followed by successful authentication activity from the same origin host.

Initial investigation identified:
- 220 counts of "User Logon Failure"
- 3 counts of "User Logon"

The activity involved user "Josh" on host "HARCOMP001" impacting host "ARDVOMP775".

A 24-hour pivot on the user account showed the user was disabled at approximately 1:30 AM CDT.

A 24-hour pivot on the origin host did not identify additional indicators of compromise (IOCs).

---

## Recommendations
- Confirm whether this activity was authorized
- If unauthorized:
  - Quarantine impacted host
  - Disable affected user account
  - Investigate for additional indicators of compromise
  - Reset associated credentials if necessary