# ADCS Tools & Resources

## Certify
### Purpose
Active Directory Certificate Services enumeration and vulnerability discovery.

### Use Cases
- Find vulnerable templates
- Enumerate certificate authorities
- Identify ESC vulnerabilities

### Example
powershell
Certify.exe find /vulnerable

### Repository
https://github.com/GhostPack/Certify


## Certipy
### Purpose
Comprehensive ADCS assessment framework.

### Use Cases
- Enumeration
- Certificate Requests
- Authentication
- ESC Exploitation

### Examples
#### Find vulnerable ADCS configurations
certipy find -vulnerable

#### Request a certificate
certipy req

#### Authenticate using certificate
certipy auth

### Repository
https://github.com/ly4k/Certipy


## ADACLScanner
Purpose
Enumerate Active Directory ACLs and permissions.

### Use Cases
Discover weak CA permissions
Identify ESC7 attack paths

### Repository
https://github.com/canix1/ADACLScanner


## Rubeus
### Purpose
Kerberos interaction and ticket management.

### Use Cases
Request TGTs
Certificate Authentication
Kerberos Abuse

### Repository
https://github.com/GhostPack/Rubeus


## Mimikatz
### Purpose
Credential extraction and authentication abuse.

### Use Cases
Kerberos Operations
Certificate-Based Authentication
Credential Analysis

### Repository
https://github.com/gentilkiwi/mimikatz


## Research References
### SpecterOps ADCS Research
https://specterops.io/blog/

### Certipy ESC15 Research
https://github.com/ly4k/Certipy/pull/228
