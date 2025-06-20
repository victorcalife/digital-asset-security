# 💾 Backup Strategy

This guide provides recommendations for designing and maintaining an effective backup plan to ensure data integrity, system resilience, and recovery readiness.

---

## 🎯 Core Objectives

- Prevent data loss from human error, system failure, or cyberattacks
- Support quick recovery during incidents (RTO / RPO alignment)
- Meet audit, compliance, and legal requirements

---

## 🧩 Backup Types

| Type             | Description                             | Example                        |
|------------------|-----------------------------------------|--------------------------------|
| Full             | Complete copy of all selected data      | Weekly full system image       |
| Incremental      | Only changed data since last backup     | Daily app data changes         |
| Differential     | Changes since last full backup          | Midweek restore points         |
| Snapshot         | Point-in-time image of VM/system        | Cloud snapshot before update   |

---

## 🔁 Recommended Practices

- **3-2-1 Rule**:  
  3 copies of data → on 2 types of storage → 1 off-site/offline
- Encrypt all backups (at rest and in transit)
- Test backup restore procedures monthly
- Version control critical documents or configs
- Automate backup processes and alerts

---

## ⚠️ Key Metrics

| Metric                   | Target                   |
|--------------------------|--------------------------|
| Recovery Point Obj (RPO) | < 1 hour                 |
| Recovery Time Obj (RTO)  | < 4 hours                |
| Backup Success Rate      | > 98%                    |
| Last Restore Test Date   | [Insert Date]            |

---

## 🛠 Tools & Providers

- **Cloud**: AWS Backup, Azure Recovery Vault, Google Snapshots  
- **Local**: Veeam, Acronis, Synology Active Backup  
- **Hybrid**: Commvault, Rubrik, Arcserve

---

## 📌 Related Practices

- [Endpoint Hardening Guide](./endpoint-hardening.md)  
- [Incident Response – Security](./incident-response-security.md)

---

[🔙 Return to Main Index](./README.md)
