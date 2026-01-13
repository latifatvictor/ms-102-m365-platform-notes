# Device Trust and Access in Microsoft 365

## What this is
This document explains how device trust works in Microsoft 365 and why it is a critical part of securing access to corporate data.

In a modern workplace, identity alone is not enough. Devices also need to be trusted.

---

## Why device trust matters
Users now work from anywhere, on many devices. Without device trust:
- Stolen credentials can be used from unmanaged devices
- Corporate data can be accessed from insecure endpoints
- Security teams lose visibility and control

By combining identity and device trust, organisations can:
- Reduce the risk of data leakage
- Enforce security without blocking productivity
- Support secure remote and hybrid work

---

## How device trust works

Microsoft 365 uses Entra ID and Intune together to determine whether a device should be trusted.

A device can be:
- Entra ID joined  
- Entra ID registered  
- Hybrid joined  

Once a device is enrolled into Intune, it can be:
- Assessed for compliance
- Configured with security policies
- Used as a signal in Conditional Access

---

## Recommended approach

### 1. Enrol devices into Intune
All corporate Windows devices should be enrolled into Intune.  
This allows:
- Policy enforcement
- Compliance checks
- Application control
- Remote management

---

### 2. Define device compliance
Compliance policies should check:
- OS version and patch level
- Encryption (BitLocker)
- Antivirus and endpoint protection
- Device health signals

Non-compliant devices should not be allowed to access sensitive services.

---

### 3. Use device trust in Conditional Access
Conditional Access should use:
- User identity
- Location
- Device compliance
- Application risk

For example:
- Allow access to Microsoft 365 only from compliant devices
- Require MFA when a device is not trusted
- Block access from unknown or risky endpoints

---

## Common pitfalls

- Allowing access from unmanaged personal devices
- Not enforcing compliance for sensitive apps
- Treating all users and devices the same
- Not reviewing device compliance reports
- Allowing legacy authentication

---

## What to validate

To confirm device trust is working:

- Check how many devices are enrolled in Intune
- Review compliance policy success rates
- Validate Conditional Access rules for device state
- Confirm BitLocker and Defender are enabled
- Monitor sign-in logs for risky device access

---

## How this supports a secure Modern Workplace

Device trust ensures that:
- Identity alone is not the only gate
- Data stays on secure, managed devices
- Users can work from anywhere safely
- IT teams maintain visibility and control

It is a core pillar of Zero Trust and Modern Workplace security.
