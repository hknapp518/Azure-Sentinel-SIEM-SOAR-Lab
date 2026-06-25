# 01 - Attack Surface

## Overview

Before detecting and responding to security threats, organizations must first establish a secure identity environment. This section documents the Microsoft Entra ID attack surface used throughout this project, including the identity, authentication, and access controls implemented prior to conducting attack simulations.

The objective is to reduce the organization's identity attack surface while generating the authentication telemetry required for Microsoft Sentinel to detect, investigate, and respond to suspicious activity.

## Architecture Diagram
<img width="637" height="1262" alt="Attack-Surface-Architecture drawio" src="https://github.com/user-attachments/assets/2bb69dfb-327a-40dd-8418-6b63895cf83c" />

---

## Objectives

* Configure a secure Microsoft Entra ID environment
* Implement layered identity security controls
* Reduce the organization's identity attack surface
* Generate authentication telemetry for Microsoft Sentinel
* Prepare the environment for identity-based attack simulations

---

## Security Controls Implemented

* Microsoft Entra ID Configuration
* Conditional Access Policies
* Multi-Factor Authentication (MFA)
* Microsoft Entra ID Identity Protection
* Role-Based Access Control (RBAC)
* Least Privilege Administration
* Sign-In Logging
* Audit Logging

---

## Folder Contents

| Document                      | Description                                                                                                                       |
| ----------------------------- | --------------------------------------------------------------------------------------------------------------------------------- |
| **Entra-ID-Configuration.md** | Documents the Microsoft Entra ID tenant configuration, authentication methods, logging configuration, and administrative roles.   |
| **Conditional-Access.md**     | Details the Conditional Access policies implemented to reduce the identity attack surface and strengthen authentication security. |


---

## Next Phase

With the Microsoft Entra ID environment configured and secured, the next phase of the project simulates identity-based attacks against the tenant. These attack scenarios generate security events that are forwarded to Microsoft Sentinel for detection engineering, automated response, and incident investigation.
