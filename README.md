# Help-Desk-Emulation-AD-USER-GROUPS-DOMAIN-PW
This lab showcases setting up Active Directory on a Windows Server virtual machine using AWS EC2. Created a domain, added users, organized groups, and practiced resetting passwords to simulate a real-world directory environment
# 🛠️ Active Directory + ServiceNow Lab (AWS EC2)

> **Simulating real-world helpdesk operations with AD DS on Windows Server 2019**  
> Hosted in the cloud ☁️ | Powered by AWS 💪 | Documented with style 😎

---

## 📦 Project Overview

| 🧩 **Component** | 📋 **Description** |
|------------------|--------------------|
| 💻 **Platform** | AWS (EC2) |
| 🏁 **OS** | Windows Server 2019 |
| 🧰 **Services** | Active Directory Domain Services, ServiceNow Developer |
| 🎯 **Goal** | Simulate daily helpdesk operations in a lab setting |

---

## 🚀 EC2 Instance Setup

1. 🖥️ Launched a **Windows Server 2019** EC2 instance using the AWS Console  
2. 🔐 Enabled **RDP access** via Security Groups (port `3389`)  
3. ⚙️ Selected **Role-Based** installation type  
4. 🧱 Installed **Active Directory Domain Services (AD DS)** via Server Manager  
5. 🏰 Promoted the instance to a **Domain Controller**  
6. 🧪 Created a test domain: `corp.local`

---

## 🔁 AD Setup Flow (Mermaid Diagram)

```mermaid
graph TD
    A[Launch EC2 Instance] --> B[Enable RDP Port 3389]
    B --> C[Install AD DS Role]
    C --> D[Promote to Domain Controller]
    D --> E[Create Test Domain: corp.local]
