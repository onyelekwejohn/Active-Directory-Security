# ADCS Attack Paths

## Overview

ADCS misconfigurations can allow attackers to:

- Escalate Privileges
- Impersonate Users
- Move Laterally
- Persist Within The Domain
- Obtain Domain Administrator Access

---

# ESC1 – Misconfigured Certificate Template Permissions

## Description

Occurs when low-privileged users can enroll in certificates that allow authentication as other users.

## Impact

- Privilege Escalation
- User Impersonation
- Domain Compromise

## Enumeration

### Certify

```powershell
Certify.exe find /vulnerable

Certipy
```Bash
certipy find -vulnerable

------------------------------------------------------------------------------

ESC3 – Enrollment Agent Abuse
Description

Abuse of Enrollment Agent templates allowing certificate enrollment on behalf of other users.

Impact
Domain Admin Impersonation
Kerberos Abuse
Privilege Escalation

Enumeration
certipy find -vulnerable

Related Tools
Certipy

ESC7 – Dangerous Certificate Authority Permissions
Description

Occurs when users have excessive permissions over the Certificate Authority.

Examples:

Manage CA
Issue and Manage Certificates

Impact
Full CA Compromise
Arbitrary Certificate Issuance
Long-Term Persistence

Related Tools
Certipy
ADACLScanner
Certify

ESC15 – Application Policy Abuse
Description

Abuse of Application Policies and EKU settings within vulnerable templates.

Impact
Certificate Authentication Abuse
LDAP Authentication
User Impersonation
Related Tools
Certipy

Additional ADCS Attack Vectors
SAN Spoofing
Misconfigured templates allow attackers to specify arbitrary identities in certificates.

NTLM Relay to ADCS
NTLM authentication can be relayed to certificate enrollment endpoints.

Vulnerable Web Enrollment
Legacy enrollment portals may expose additional attack surfaces.

Certificate Persistence
Certificates often remain valid after password changes.
This allows attackers to maintain access longer than traditional credential theft.
