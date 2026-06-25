## Conditional Access Policies

Conditional Access policies were implemented to strengthen identity security, enforce Zero Trust principles, and reduce the organization's overall attack surface. Each policy was designed to address a specific authentication risk while balancing security and usability.

### Configured Policies

#### Block Legacy Authentication

Legacy authentication protocols such as POP, IMAP, and SMTP AUTH do not support modern authentication or Multi-Factor Authentication (MFA). Blocking these protocols reduces the risk of password spray, credential stuffing, and brute-force attacks that commonly target legacy authentication.

#### External User Access Control

External guest accounts introduce additional security risk because they exist outside the organization's direct administrative control. This policy limits guest access, enforces authentication requirements, and helps prevent unauthorized access to sensitive Microsoft 365 and Azure resources.

#### Location-Based Access Control

Restricts authentication attempts originating from countries or geographic regions that are not associated with normal business operations. This reduces exposure to unauthorized access attempts from unexpected or high-risk locations.

#### Privileged Administrator Protection

Applies additional authentication requirements and access restrictions to privileged administrative accounts. Administrative identities represent high-value targets and require stronger security controls to reduce the risk of privilege escalation and administrative account compromise.

#### Require MFA for Clinical Users

Requires Multi-Factor Authentication (MFA) for all members of the Clinical Users security group before access is granted to organizational resources. MFA significantly reduces the risk of account compromise resulting from stolen or reused credentials.

#### Sign-In Risk Protection

Uses Microsoft Entra ID Identity Protection to evaluate authentication risk in real time. High-risk sign-in attempts can be blocked, challenged with MFA, or require password reset based on the configured policy.

---

Several Conditional Access policies were initially deployed in Report-only mode to evaluate policy impact, validate policy logic, and identify potential user disruptions before enforcement. Policies were transitioned to On after testing confirmed the expected behavior. Multi-Factor Authentication (MFA) was enabled immediately because it provides a significant security improvement with minimal operational overhead.

> **Figure 1:** Conditional Access Policy Overview
<img width="1826" height="782" alt="image" src="https://github.com/user-attachments/assets/3b98a674-11c3-4d9c-8277-f428b999e4cc" />


> **Figure 2:** Microsoft Entra ID Conditional Access policies configured for the lab environment.


<img width="1706" height="804" alt="image" src="https://github.com/user-attachments/assets/f22ed27c-4835-44e9-ad6a-68229d6c9736" />

