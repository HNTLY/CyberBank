# Active Directory
## Introduction
AD was first introduced as part of Windows Server 2000 after having it previewed in 1999 with it being expanded and improved in Windows Server 2003 such as including AD Federation Services.
Initially, it focused on centralized domain management but has now become an umbrella title lots of directory-based identitiy-related servcies.
AD is now included with most Windows Server OS's.

## Overview
AD allows administrators to manage devices, users, domains and objects within a network.
AD provides multiple services:
- DS (Domain Services)
    - Plays the role of authenticating and authorising users and devices on the network.
    - A server running the AD DS is known as the domain controller
- CS (Certificate Services)
    - Builds Public Key Infrastructure (PKI) and provides public key crypto, digital certificates and digital signatures
- FS (Federation Services)
    - Performs Single Sign On (SSO) and provides users authentication access to a variety of compatible systems and applications.
- RMS (Rights Management Services)
    - Protects sensitive data with rights management and access policy enforcement.
    - Controls access to information such as: documents, emails and web pages
    
AD will categorise objects by name and attribute e.g users name along with associated information such as SSH keys or passwords etc

## Abbreviations and Definitions

Keyword | Definition
--- | ---
AD | Active Directory
Containers | Similar to OU's but GPO's cannot be applied
Domain | Group of objects e.g users
Forest | Group of multiple trees
GPO | Group Policy Objects
LDAP | Lightweight Directory Access Protocol
OU | Organisational Unit. Organises users, groups and devices and ensures each object is unique e.g no 2 users with same username
Tree | One or more domains grouped together. Uses a trust hierachy e.g first domain trusts third domain without needing explicit trust
