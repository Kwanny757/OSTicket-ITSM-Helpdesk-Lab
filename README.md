# Enterprise IT Help Desk & ITSM Lab Deployment
**Platform:** osTicket v1.18.x | **Environment:** Windows 11 Enterprise (Oracle VM VirtualBox) | **Stack:** XAMPP (Apache, MariaDB/MySQL, PHP)

📄 **[Download Full 11-Page Portfolio PDF](./Dekwan%20Harris%20Help%20Desk%20OSTicket%20Portfolio.pdf)**

---

## 📌 Project Overview
Built a fully functional, virtualized IT Service Management (ITSM) ticketing environment from scratch using Oracle VM VirtualBox, XAMPP, and osTicket. Implemented Role-Based Access Control (RBAC), multi-tiered departmental escalation paths, SLA policies, and simulated end-to-end incident lifecycles aligned with ITIL Service Operation standards.

---

## 🛠️ Technologies & Core Competencies
* **Virtualization & OS:** Oracle VM VirtualBox, Windows 11 Enterprise (8 GB vRAM, 4 vCPUs)
* **Web & DB Infrastructure:** Apache, MariaDB/MySQL via phpMyAdmin (`dekwan_osticket` database), PHP module validation
* **IT Service Management (ITSM):** ITIL Service Operation framework, Incident Lifecycles, SLA Policies, Role-Based Access Control (RBAC)
* **Technical Support Triage:** Active Directory account lockouts, Hardware diagnostics (SAS disk replacement & RAID parity rebuilds), NTFS/Share permission inheritance & Tier 2 escalations

---

## ⚙️ Infrastructure & Administrative Setup
1. **Virtual Machine Provisioning:** Allocated an isolated Windows 11 Enterprise VM configured with 8 GB RAM and 4 virtual processor cores.
2. **Database & Web Server Stack:** Initialized Apache and created a dedicated relational database (`dekwan_osticket`) via phpMyAdmin.
3. **RBAC & Department Queues:** Defined least-privilege permission roles across Desktop Support, Maintenance, and Systems Administration teams.
4. **SLA Plan Engine:**
   * **SEV-1 (Emergency / Critical):** 1-hour response / 4-hour resolution for critical system and storage outages.
   * **Default SLA:** Standard business-hours resolution for routine access requests.

---

## 🎫 Simulated Incident Lifecycles

### 1. Account Lockout & Identity Verification (Ticket #900699)
* **Issue:** User locked out after repeated failed logins.
* **Resolution:** Verified user identity via employee ID, unlocked Active Directory account, issued a temporary one-time password with mandatory change at next logon, and confirmed successful access.

### 2. Critical Storage Outage / SEV-1 Emergency (Ticket #639432)
* **Issue:** Primary departmental shared storage array offline following a power surge.
* **Resolution:** Ingested emergency alert, dispatched on-site technician, replaced failed SAS drives with cold spares, executed RAID parity reconstruction, and restored full database services.

### 3. File Share Permission Triage & Escalation (Ticket #148299)
* **Issue:** User denied access to departmental payroll share following team transfer.
* **Resolution:** Executed Tier 1 diagnostic triage, verified Active Directory group memberships, confirmed missing security group permissions, and smoothly escalated to Systems Administration with full internal handover notes.

---

## 📂 Full Documentation
For complete step-by-step screenshots and administrative configuration logs, review the full [Portfolio Document](./Dekwan%20Harris%20Help%20Desk%20OSTicket%20Portfolio.pdf).
