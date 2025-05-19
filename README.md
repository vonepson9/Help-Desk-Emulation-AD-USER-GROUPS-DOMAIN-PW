# Help-Desk-Emulation-AD-USER-GROUPS-DOMAIN-PW
This lab showcases setting up Active Directory on a Windows Server virtual machine using AWS EC2. Created a domain, added users, organized groups, and practiced resetting passwords to simulate a real-world directory environment
# 🔐 Active Directory Lab on AWS EC2

> **Hands-on Identity & Access Management Lab**  
> Simulated enterprise-level user management using a Windows Server virtual machine hosted on AWS EC2 ☁️🖥️

---

## 🧠 Project Overview

This lab showcases the setup and configuration of **Active Directory** in a cloud-hosted Windows Server VM via **AWS EC2**. The goal was to simulate real-world scenarios around identity management and group policies.

### 🛠️ What I Did:
- ✅ Deployed a **Windows Server 2019** EC2 instance on AWS
- 🏗️ Installed **Active Directory Domain Services (AD DS)**
- 🌐 Created a custom **domain**
- 👤 Added users and assigned them to **organizational groups**
- 🔁 Practiced **resetting passwords** and managing access
- 🔒 Simulated basic **access control** in an enterprise environment

---

## 📊 AD Setup Flow (Mermaid Diagram)

```mermaid
graph TD
    A[Launch EC2 Instance] --> B[Install Windows Server]
    B --> C[Install AD DS Role]
    C --> D[Promote to Domain Controller]
    D --> E[Create Domain]
    E --> F[Add Users]
    F --> G[Create Groups]
    G --> H[Reset Passwords]

