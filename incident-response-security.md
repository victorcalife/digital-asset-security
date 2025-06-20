# 🚨 Incident Response – Security

This document outlines the standard operating procedures for identifying, managing, and recovering from information security incidents.

---

## 🎯 Objectives

- Minimize impact of security breaches
- Ensure rapid containment and recovery
- Preserve evidence for audit or legal use
- Improve organizational resilience through learning

---

## 🚦 Incident Stages

### 1. 🔍 Detection & Triage
- Automated alerts (EDR, SIEM, WAF, email gateway)
- User-reported anomalies (phishing, abnormal behavior)
- Initial classification by severity and asset affected

### 2. 🧯 Containment
- Isolate affected endpoints or services
- Revoke compromised credentials or access
- Disable integrations if needed (e.g., CI/CD pipelines)

### 3. 🔄 Eradication & Recovery
- Patch vulnerabilities exploited
- Clean infected systems
- Restore from last known-good backup
- Confirm threat is neutralized

### 4. 🧾 Postmortem & Reporting
- Document root cause and timeline
- Update playbooks and controls
- Share learnings with stakeholders
- Notify legal/compliance if required

---

## 📌 Roles & Responsibilities

| Role                | Responsibility                                |
|---------------------|-----------------------------------------------|
| Incident Commander  | Coordinates response, approves actions        |
| Security Analyst    | Investigates and triages incident             |
| IT Ops              | Supports containment and recovery actions     |
| Communications Lead | Internal/external notifications               |
| Legal/Compliance    | Regulatory and evidence handling              |

---

## 🛠 Tools to Support IR

- SIEM: Splunk, Graylog, Microsoft Sentinel  
- EDR: CrowdStrike, SentinelOne, Defender ATP  
- Ticketing: Jira, ServiceNow, FreshService  
- Forensics: Velociraptor, KAPE

---

## 📌 Related Practices

- [Backup Strategy](./backup-strategy.md)  
- [Credential Management](./credential-management.md)

---

[🔙 Return to Main Index](./README.md)
