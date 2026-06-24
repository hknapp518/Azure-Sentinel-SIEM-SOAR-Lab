Applied Conditional Access Policies to strengthen identity protection and reduce organizational attack surface.

Configured policies included:

- Block Legacy Authentication - Legacy protocols such as POP,IMAP, and SMTP AUTH do not support MFA and are frequently targeted by password spray attacks.
- External User Access Control - External guest accounts introduce additional risk because they are outside the organization's direct admin control. This is to limit guest permissions, enforce auth requriments, and reduce likelihood of unathorized access to sensitive resources. 
- Location-Based Access Control - Restrics sign-ins from countries or geogrpahic regions that are not assosciated with the business operations. Reduces exposure to unathorized access attempts from high risk or unexpected locations.
- Privileged Admin Access Protection
- Require MFA for All Clinical Users
- Sign-In Risk Protection

Several policies were initially deployed in Report-only mode to evaluate user impact, validate policy logic, and reduce the risk of unintended access disruptions before enforcement. While MFA was enabled due to it being a free security improvement.

<img width="1706" height="804" alt="image" src="https://github.com/user-attachments/assets/f22ed27c-4835-44e9-ad6a-68229d6c9736" />

