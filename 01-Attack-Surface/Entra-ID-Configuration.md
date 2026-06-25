# Microsoft Entra ID Configuration

## Overview

Microsoft Entra ID serves as the identity provider for this lab environment. It manages user authentication, role-based access control (RBAC), security groups, and authentication logging that supports the Microsoft Sentinel SIEM environment used throughout this project.

---

## Tenant Configuration

The lab was deployed using a Microsoft 365 Developer tenant with Microsoft Entra ID as the central identity platform.

Configuration included:

* Microsoft Entra ID P2 licensing
* Test user accounts
* Security groups
* Administrative roles
* Multi-Factor Authentication (MFA)
* Authentication logging
 

---

## Security Groups

Security groups were created to support role-based access control (RBAC) and organizational separation of duties.

Example groups:

* Clinical Users
* Clinical Data Team
* Research Leads
* Security & Compliance
* IT
* External Users

Permissions were assigned through security groups to support least privilege and simplify identity administration.

*Insert Security Groups screenshot*

---

## Administrative Roles

Administrative roles were assigned using the principle of least privilege to separate administrative responsibilities.

Example roles:

* Global Administrator
* Security Administrator
* User Administrator

*Insert Roles screenshot*

---

## Authentication & Logging

Authentication logging was enabled to capture user sign-in activity and administrative events.

Logs configured:

* Sign-In Logs
* Audit Logs

These logs are later ingested into Microsoft Sentinel for monitoring, detection, and incident investigation.

*Insert Sign-In Logs screenshot*

---

## Summary

Microsoft Entra ID provides the identity foundation for this project by managing authentication, authorization, and logging. These capabilities support the Conditional Access policies and Microsoft Sentinel detections implemented throughout the remaining phases of the lab.

