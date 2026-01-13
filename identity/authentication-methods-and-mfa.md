# Authentication Methods and MFA in Microsoft 365

## What this is
This document describes how authentication methods and multi-factor authentication (MFA) should be designed and managed in Microsoft 365 using Entra ID.

Authentication is the first line of defence for all Microsoft 365 services.

---

## Why it matters
Weak authentication is one of the most common causes of account compromise.

Strong authentication:
- Protects against password theft
- Reduces phishing impact
- Supports Zero Trust access
- Enables secure remote work

---

## Authentication methods in Entra ID

Microsoft 365 supports multiple authentication methods, including:
- Password
- Microsoft Authenticator
- FIDO2 security keys
- SMS and voice
- Temporary Access Pass
- Certificate-based authentication

Not all methods provide the same level of security.

---

## Recommended approach

### 1. Prefer phishing-resistant methods
Where possible, use:
- Microsoft Authenticator (push or number matching)
- FIDO2 security keys
- Certificate-based authentication

These significantly reduce the risk of phishing.

---

### 2. Enforce MFA for all users
MFA should be required for:
- All user sign-ins
- All admin sign-ins (stronger controls)

Conditional Access should be used to:
- Enforce MFA
- Apply stronger requirements for higher-risk access

---

### 3. Use Temporary Access Pass for onboarding
Temporary Access Pass allows:
- Secure first-time sign-in
- Device registration
- Passwordless setup

This reduces reliance on insecure temporary passwords.

---

### 4. Protect privileged access
Admins should:
- Use separate admin accounts
- Always be required to use MFA
- Use stronger authentication methods where possible

---

## Common mistakes

- Allowing SMS as the primary MFA method
- Not enforcing MFA for all users
- Not protecting service and admin accounts
- Using legacy authentication
- Allowing long-term bypasses

---

## What to validate

To ensure authentication is secure:
- Check MFA coverage
- Review authentication method usage
- Block legacy authentication
- Review risky sign-ins
- Validate admin authentication strength

---

## How this supports a secure Modern Workplace

Strong authentication ensures:
- Users can work from anywhere safely
- Devices and apps can be trusted
- Identity-based attacks are reduced
- Microsoft 365 remains secure and usable

It is a core foundation of Zero Trust and Modern Workplace security.
