# Active Directory Certificate Services (ADCS)

## Overview

Active Directory Certificate Services (ADCS) is Microsoft's Public Key Infrastructure (PKI) implementation used to issue and manage digital certificates within Active Directory environments.

ADCS helps provide:

- Authentication
- Encryption
- Digital Signatures
- Secure Communications
- Identity Verification

## ADCS Components

### Certificate Authority (CA)

Responsible for issuing and managing certificates.

### Certificate Templates

Define:

- Certificate permissions
- Enrollment rights
- Key usage
- Subject naming

### Web Enrollment

Allows certificate requests through a web interface.

### Network Device Enrollment Service (NDES)

Issues certificates to network devices.

### Online Responder

Provides certificate validation services.

## ADCS Integration with Active Directory

ADCS integrates with:

- Active Directory Users
- Computer Accounts
- Security Groups
- Group Policy
- Kerberos Authentication

## Common Certificate Use Cases

### Authentication

- Smart Card Logons
- VPN Authentication
- Wi-Fi Authentication

### Encryption

- TLS/SSL
- EFS
- S/MIME

### Code Signing

- Scripts
- Applications
- Executables

### Digital Signatures

- Documents
- Email Signing

## Common ADCS Weaknesses

- Weak Template Permissions
- SAN Spoofing
- Excessive Enrollment Rights
- Vulnerable Web Enrollment
- NTLM Relay
- Deprecated Templates
- Weak EKU Configuration
- Dangerous CA Permissions

## Learning Objectives

- Understand ADCS Architecture
- Enumerate Certificate Templates
- Identify Misconfigurations
- Assess Certificate Authority Security
- Understand ESC Attack Paths

