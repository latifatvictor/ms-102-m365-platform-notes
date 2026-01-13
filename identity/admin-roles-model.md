# Microsoft 365 Admin Roles Model

## What this is
This document describes a practical approach to managing administrative roles in Microsoft 365 and Entra ID, using the principle of least privilege to reduce risk while still enabling teams to work effectively.

In most environments, the biggest identity risk is not external attackers, but excessive or unmanaged administrative access.

---

## Why this matters
Admin roles control everything from user access to security settings, data protection, and device management. Poor role management leads to:
- Higher risk of account compromise
- Audit and compliance issues
- Uncontrolled changes to production systems
- Lack of accountability

A clear admin roles model improves:
- Security posture  
- Operational stability  
- Change traceability  
- Confidence in the platform  

---

## Recommended approach

### 1. Use role-based separation
Avoid using Global Administrator for day-to-day work.

Typical role split:
- Global Administrator (very limited, emergency only)
- Identity Administrator
- Endpoint Administrator
- Security Administrator
- Exchange / Collaboration Administrator
- Compliance Administrator

Each admin should only have the roles required for their responsibilities.

---

### 2. Enforce least privilege
Admin access should be:
- Time-bound  
- Role-specific  
- Audited  

Where possible:
- Use Privileged Identity Management (PIM)
- Require approval for high-risk roles
- Require MFA for all admin access

---

### 3. Separate admin identities
Admins should have:
- A normal user account for daily work
- A separate admin account for privileged actions

This reduces the risk of phishing and token theft impacting admin access.

---

### 4. Control and review access
All admin roles should be:
- Documented
- Approved
- Reviewed regularly

A quarterly review should confirm:
- Who has access
- Why they have it
- Whether it is still required

---

## Common pitfalls

- Too many Global Administrators
- No separation between admin and user accounts
- No expiry or review of admin access
- Shared admin accounts
- No MFA on admin roles

These issues are extremely common and significantly increase risk.

---

## What to validate

To confirm your admin model is working:

- Check how many Global Administrators exist
- Review all role assignments in Entra ID
- Confirm MFA is enforced for admin roles
- Confirm PIM is enabled where available
- Ensure admin activity is logged and monitored

---

## How this supports a secure Modern Workplace

A well-managed admin roles model:
- Protects Microsoft 365 from internal and external threats
- Supports audit and compliance requirements
- Reduces the blast radius of account compromise
- Enables controlled, reliable platform changes

This is a foundation for everything else in identity, endpoint, and security.
