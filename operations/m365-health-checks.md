# Microsoft 365 Health Checks

## What this is
This document describes a practical approach to monitoring and validating the health of Microsoft 365 services from an operations and service ownership perspective.

It is designed to ensure the platform remains secure, reliable, and fit for purpose in a production environment.

---

## Why health checks matter
Microsoft 365 is a business-critical platform. If it becomes unstable or insecure:
- Users cannot work
- Data is at risk
- Incidents increase
- Trust in IT decreases

Regular health checks allow teams to:
- Detect issues early
- Reduce incidents
- Maintain security posture
- Support consistent service delivery

---

## Key health check areas

### 1. Identity and Access
Validate:
- MFA enforcement for all users and admins
- Conditional Access policy health
- Sign-in failure and risk trends
- Admin role assignments
- Privileged access usage

---

### 2. Endpoint and Device Trust
Validate:
- Number of devices enrolled in Intune
- Compliance rates across devices
- Endpoint protection status
- Windows update compliance
- Device trust used in Conditional Access

---

### 3. Security Controls
Validate:
- Defender alert trends
- Email threat protection status
- Cloud app activity and risky sign-ins
- Data loss prevention events
- Security configuration drift

---

### 4. Service Reliability
Validate:
- Microsoft 365 service health
- Incident and outage trends
- Support ticket volume
- Root cause themes
- Change success rates

---

### 5. Governance and Compliance
Validate:
- Admin access reviews
- Guest user reviews
- Data retention and protection policies
- Audit log availability
- Policy ownership and documentation

---

## Recommended cadence

- Daily:  
  - Service health  
  - Security alerts  
  - Sign-in anomalies  

- Weekly:  
  - Device compliance  
  - Identity trends  
  - Support volumes  

- Monthly:  
  - Admin role review  
  - Conditional Access review  
  - Governance checks  

---

## Common gaps

- Health checks done only after incidents
- No ownership of security signals
- No reporting to stakeholders
- No regular admin or device reviews
- Changes made without impact assessment

---

## How this supports service ownership

Health checks turn Microsoft 365 from a collection of tools into a managed platform.

They:
- Reduce firefighting  
- Improve stability  
- Support security  
- Provide visibility to leadership  

This is what separates a platform owner from a ticket resolver.
