# 🧬 Code Repository Protection

This guide provides security practices to safeguard source code, configuration files, and version-controlled assets hosted in Git-based repositories.

---

## 🚨 Core Risks

- Exposure of hardcoded secrets (API keys, passwords, tokens)
- Unauthorized access to private repositories
- Accidental or malicious code deletion
- Sensitive data leaks via commits

---

## 🔐 Best Practices

### 1. 🔒 Repository Access Control
- Use **private repositories** by default
- Enforce **MFA** for all Git platform users
- Apply **least privilege** access (e.g., read-only for QA, write for Devs)
- Use **teams/groups** for permission management, not individuals

### 2. 📜 Commit Hygiene
- Reject commits with secrets using tools like `gitleaks`, `truffleHog`
- Enforce commit message standards via hooks or CI
- Prohibit `force push` to main branches

### 3. 🧪 Branch Protection Rules
- Enable **required pull request reviews**
- Block direct commits to `main`, `master`, or release branches
- Require **status checks** before merging (e.g., CI build, lint)

### 4. 🔍 Audit & Monitoring
- Enable **audit logs** for repository events
- Periodically review access and permissions
- Track branch deletions, force pushes, and repository cloning

---

## 🛠 Recommended Tools

| Function         | Tool Example                     |
|------------------|----------------------------------|
| Secrets Scanner  | Gitleaks, TruffleHog             |
| CI Protection    | GitHub Actions, GitLab CI        |
| Access Reviews   | GitHub Audit Log, GitLab Monitor |
| Repo Backup      | `git bundle`, CodeGuard          |

---

## 📌 Related Practices

- [Credential Management](./credential-management.md)  
- [Endpoint Hardening Guide](./endpoint-hardening.md)

---

[🔙 Return to Main Index](./README.md)
