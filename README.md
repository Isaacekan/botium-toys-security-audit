# Botium Toys  Internal Security Audit & Risk Assessment

Internal security audit and controls/compliance checklist for **Botium Toys**, a fictional small U.S. toy retailer, completed as a hands-on exercise in the **Google Cybersecurity Professional Certificate** (Coursera).

> **Note:** This is a training exercise based on a fictional company scenario provided by the course — not a live client engagement. It's shared here to demonstrate applied understanding of the NIST Cybersecurity Framework, control categories, and compliance requirements.

**Prepared by:** Isaac Ekaniyere
**Framework referenced:** NIST Cybersecurity Framework (CSF)  Identify function

📄 Full write-up: [`Botium-Toys-Internal-Security-Audit.pdf`](./Botium-Toys-Internal-Security-Audit.pdf)

## Scope & Goals

Assess all assets managed by Botium Toys' IT department and complete a controls and compliance checklist to determine what needs to be implemented to improve the company's security posture, using the **NIST CSF — Identify** function as the starting point.

## Risk Summary

**Risk score: 8/10**  driven by a lack of implemented controls and inconsistent adherence to compliance best practices, particularly around cardholder data protection and access control.

## Controls Checklist

| Control | Status | Rationale |
|---|:---:|---|
| Least privilege |  No | All employees currently have access to internally stored data, including cardholder data and PII/SPII. |
| Disaster recovery plan |  No | No DR plan exists, and no backups of critical data. |
| Password policy |  No | Policy exists but is nominal — doesn't meet minimum complexity standards. |
| Account management (centralized password mgmt) |  No | No centralized system enforcing requirements; resets rely on manual tickets. |
| Separation of duties |  No | Not implemented. |
| Firewall |  Yes | Configured with a defined rule set to block malicious traffic. |
| IDS/IPS |  No | Not installed. |
| Encryption |  No | Cardholder data is stored/transmitted without encryption. |
| Backups |  No| None in place. |
| Antivirus |  Yes| Installed and monitored regularly. |
| Physical controls (locks, CCTV, fire detection) |  Yes| Sufficient locks, up-to-date CCTV, functioning fire systems. |

## Compliance Checklist

| Area | Status | Rationale |
|---|:---:|---|
| PCI DSS (payment card data) |  No | Cardholder data unencrypted and not access-restricted. |
| SOC (data integrity & availability) |  Yes | Availability ensured; integrity controls in place. |
| GDPR (EU customers) | Yes | 72-hour breach notification process in place; documented privacy policies. |

## Recommendations

- Implement encryption (at rest & in transit) for cardholder data — highest priority given online payment processing
- Adopt least privilege and separation of duties for access to PII/SPII and cardholder data
- Deploy a centralized password management system with enforced complexity requirements
- Build and test a disaster recovery plan, supported by regular backups
- Deploy an IDS/IPS alongside the existing firewall
- Formalize a maintenance schedule for legacy systems

## Skills Demonstrated

`Risk Assessment` `NIST CSF` `PCI DSS` `GDPR` `Controls Testing` `Security Audit` `GRC`
