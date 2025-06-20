# 🔑 Credential Management

This document outlines best practices for managing passwords, tokens, API keys, certificates, and other credentials across systems and environments.

---

## 🔒 Core Guidelines

- **No hardcoded credentials** in code, scripts, or configuration files.
- Use **vaulted storage systems** (e.g., HashiCorp Vault, AWS Secrets Manager, Azure Key Vault).
- Rotate sensitive credentials **at least every 90 days**, or immediately after exposure.
- Ensure all credentials are tied to a **named entity (user or system)** and not shared.
- Apply **multi-factor authentication (MFA)** for all privileged and remote access.

---

## 🧰 Tools & Mechanisms

| Type            | Recommended Tool(s)                 |
|-----------------|-------------------------------------|
| Secrets Vault   | HashiCorp Vault, AWS Secrets Manager |
| Password Vault  | Bitwarden, 1Password, KeePassXC     |
| Token Manager   | GitHub Secrets, GitLab CI Variables |
| MFA Provider    | Duo, Authy, Okta, Microsoft Auth     |

---

## ⚙️ Automation Tips

- Integrate secrets into CI/CD pipelines using environment variables.
- Use infrastructure-as-code to provision and rotate secrets securely.
- Implement alerts for credentials nearing expiration.

---

## 🚨 Incident Response

If a credential is compromised:

1. **Revoke immediately** and rotate the secret.
2. Identify affected systems/users.
3. Audit recent usage logs.
4. Update access controls and communicate with stakeholders.
5. Document the event for future prevention.

---

## 📌 Related Practices

- [Access Control Policy](./access-control-policy.md)  
- [Code Repository Protection](./code-repo-protection.md)

---

[🔙 Return to Main Index](./README.md)
