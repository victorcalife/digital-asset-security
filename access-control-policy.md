# 🛡 Access Control Policy

This document defines the principles and practices for managing access to corporate systems, applications, and infrastructure in a secure, traceable, and compliant manner.

---

## 🔑 Access Principles

- **Least Privilege**: Users must have only the access necessary to perform their duties.
- **Role-Based Access Control (RBAC)**: Access is assigned based on job role, not individual preferences.
- **Separation of Duties**: Critical tasks are split to avoid single points of control or fraud.
- **Just-in-Time Access**: Temporary access is granted for critical needs and automatically revoked.

---

## 🧩 Access Types

| Type                 | Examples                         | Control Mechanism                |
|----------------------|----------------------------------|----------------------------------|
| User Access          | Email, ERP, CRM                  | RBAC, MFA                        |
| Admin Access         | Servers, Databases, Firewalls    | Bastion Host, Approval Flow      |
| API/System Access    | Integrations, CI/CD pipelines    | Tokens, Secrets Vault            |
| Temporary Access     | Support access, incidents        | Time-restricted with logging     |

---

## 🔍 Monitoring & Auditing

- All access requests are logged and reviewed weekly.
- Admin/root sessions are session-recorded and retained for 90 days.
- Periodic access reviews (at least quarterly) are conducted with system owners.

---

## ⚠️ Violations & Remediation

- Unauthorized access attempts are logged and escalated immediately.
- Breaches of policy can result in access revocation, disciplinary action, and incident reporting.

---

## 📌 Related Practices

- [Credential Management](./credential-management.md)  
- [Incident Response – Security](./incident-response-security.md)

---

[🔙 Return to Main Index](./README.md)
