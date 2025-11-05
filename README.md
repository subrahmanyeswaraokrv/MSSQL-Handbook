# MSSQL Database Repository 📦

This repository contains all documentation, scripts, configuration files, monitoring tools, and standard operating procedures (SOPs) related to **Microsoft SQL Server** (MSSQL) database administration and activities.

---

## 📁 Repository Structure

mssql-repo/
├── backups/ # Backup scripts and schedules (full, diff, log)
├── monitoring/ # Monitoring tools, queries, and alerts (e.g., disk, CPU, blocking)
├── maintenance/ # Index maintenance, statistics updates, integrity checks
├── performance/ # Performance tuning queries, execution plans
├── security/ # Login audit, permissions, roles, and password rotation
├── high_availability/ # Always On, log shipping, replication configs
├── migration/ # Migration checklists, scripts, and logs
├── scripts/ # Useful administrative T-SQL scripts
├── upgrades/ # Version upgrade plans and rollback strategies
├── logs/ # DB snapshot logs, audit trails (non-sensitive)
├── docs/ # SOPs, architecture diagrams, documentation
└── README.md # Repository overview

yaml
Copy
Edit

---

## 🎯 Objectives

- Maintain a **centralized repository** for MSSQL DBA activities.
- Enable **version-controlled** database operations.
- Standardize **backup, monitoring, and security** processes.
- Track and document **incidents, changes**, and **migrations**.

---

## 🔧 Common Tasks Covered

| Category              | Description                                           |
|----------------------|-------------------------------------------------------|
| Backup & Restore     | Scripts for full, diff, and transaction log backups   |
| Performance Tuning   | Long-running queries, blocking sessions, deadlocks   |
| Security Management  | Logins, roles, audits, and permission scripts         |
| Maintenance Jobs     | Index rebuilds, DBCC CHECKDB, update stats            |
| Monitoring & Alerts  | CPU/memory alerts, job failures, disk space checks    |
| HA/DR                | Always On setup, failover testing plans               |
| Upgrades             | SQL Server version upgrade steps and rollback docs    |
| Auditing             | Capture login attempts, permission changes            |

---

## 🧪 Prerequisites

- SQL Server 2016 or higher (can be customized)
- SQLCMD / SSMS installed
- PowerShell 5+ (for automation scripts)
- Git for version control

---

## 📖 Usage

```bash
# Clone the repository
git clone https://github.com/your-org/mssql-repo.git
cd mssql-repo

# Run a backup script
sqlcmd -S YOUR_SERVER -i backups/backup_full.sql
🛡️ Security & Compliance
No production passwords should be stored in plain text.

Follow your organization's least privilege policy.

Review and rotate credentials periodically.

Audit scripts available under security/.

📚 References
SQL Server Docs

SQL Server Monitoring with Prometheus

DBA Checklist - Brent Ozar

👨‍💻 Maintainers
Venkata Subrahmanyeswarao Karri – Sr. Database Architect

Contact: subrahmanyeswaraokarri@gmail.com | Location: Hyderabad,India
