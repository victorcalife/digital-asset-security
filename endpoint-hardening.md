# 💻 Endpoint Hardening Guide

This guide outlines key practices to secure laptops, desktops, and mobile devices used by employees or contractors, reducing risks of data loss and endpoint compromise.

---

## 🔒 Core Protection Areas

### 1. 🔐 Device Access
- Enforce full-disk encryption (BitLocker, FileVault)
- Require strong passwords or biometric login
- Auto-lock screen after 5 minutes of inactivity
- Enable remote wipe for lost/stolen devices

### 2. 🔄 Patch Management
- Automate OS and software updates
- Set weekly patch windows for non-critical updates
- Urgent patches must be applied within 48h of release

### 3. 🛡 Antivirus & EDR
- Use next-gen antivirus + endpoint detection & response (EDR)
- Preferred: CrowdStrike, SentinelOne, Microsoft Defender for Endpoint
- Monitor and respond to anomalies in real time

### 4. 🧑‍💻 Admin Rights
- Users should not have local admin privileges by default
- Elevation of privilege must be temporary and logged
- All admin access must be justified and auditable

### 5. 🌐 Network Control
- Block access to insecure Wi-Fi networks
- Route all traffic via VPN or secure proxy for remote users
- Segment internal networks for critical systems

---

## 🧰 Recommended Tools

| Area             | Tool Example                        |
|------------------|-------------------------------------|
| EDR              | CrowdStrike, Microsoft Defender     |
| Patching         | WSUS, Intune, ManageEngine          |
| Remote Wipe      | JAMF, Intune, Knox Manage           |
| Policy Enforce   | GPO, JAMF, MDM Profiles             |

---

## 📌 Related Practices

- [Code Repository Protection](./code-repo-protection.md)  
- [Backup Strategy](./backup-strategy.md)

---

[🔙 Return to Main Index](./README.md)
