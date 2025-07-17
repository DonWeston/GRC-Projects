# GRC-Projects
This is a Access control policy for a GRC Project
# Access Control Policy

**Version:** 1.0  
**Effective Date:** 07-17-2025 
**Last Reviewed:** 07-17-2025

## 1. Purpose
Define how access to systems and data is properly granted, reviewed, and revoked to protect company assets.

## 2. Scope
Applies to all employees, contractors, and systems (cloud apps, on‑prem servers, network devices).

## 3. Policy Statements
- Access is granted based on the **principle of least privilege**.
- **Multi-Factor Authentication (MFA)** is required for all administrative access.
- User access is **reviewed quarterly** by IT and HR.
- Access changes (onboarding, promotion, termination) must be logged and actioned within **2 business days**.

## 4. Roles & Responsibilities
- **IT Team**: Implements, monitors, and revokes access.
- **HR Team**: Communicates staff changes to IT promptly.
- **Employees**: Use credentials responsibly and report suspicious activity.

## 5. Compliance & Enforcement
Non‑compliance may result in disciplinary action or termination. Exceptions must be formally approved by the CISO.

## 6. Definitions
- **Least Privilege**: Only necessary permissions for job duties.
- **MFA**: Two or more independent authentication factors.

---

📌 **Lab Task**:  
- Replace the placeholders with actual dates.  
- Add/edit statements to reflect your fictional company (e.g., “procore.project.com requires SSO”).

---

## 🧾 2. Risk Register  (Markdown & Table)

Good for a file named `risk-register.md`:

```markdown
# Risk Register: Rogue Construction

| Risk ID | Asset / Process            | Risk Description                 | Impact | Likelihood | Risk Rating | Controls In Place        | Controls Needed                   | MITRE / Threat Vector                                     |
|--------|-----------------------------|----------------------------------|--------|-------------|-------------|--------------------------|------------------------------------|-----------------------------------------------------------|
| R-001  | Office Email (M365)         | Phishing → credential theft      | High   | Likely      | High        | Spam filters; basic training | Phishing simulations; MFA         | MITRE T1566.001 – Spearphishing Attachment                |
| R-002  | Payroll System (Gusto)      | Weak login credentials           | Medium | Possible    | Medium      | Complex password rules      | Enforce MFA; audit logs           | Credential Access                                         |
| R-003  | Mobile devices on site      | Loss or theft → data leak        | High   | Likely      | High        | Screen lock; inventory list | Full-disk encryption; remote wipe | Physical access → data exfiltration                      |
| R-004  | Procore SaaS                | Unauthorized file access         | High   | Possible    | Medium      | Role-based access           | Quarterly access review          | Insider misuse; external account compromise              |
| R-005  | Vendor invoice processing   | Malware in email attachments     | High   | Possible    | High        | Email scanning              | End-user training; sandbox email | MITRE T1566.002 – Phishing Link                          |
