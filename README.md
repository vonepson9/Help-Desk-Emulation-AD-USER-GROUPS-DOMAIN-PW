# Help-Desk-Emulation-AD-USER-GROUPS-DOMAIN-PW
This lab showcases setting up Active Directory on a Windows Server virtual machine using AWS EC2. Created a domain, added users, organized groups, and practiced resetting passwords to simulate a real-world directory environment
# 🧠 Active Directory Helpdesk Lab on AWS 🚀

> **Simulating real-world helpdesk ops in a cloud-hosted lab**  
> 🖥️ Powered by AWS EC2 | 🏰 Built with Active Directory | 🎫 Integrated with ServiceNow

---

## 📊 Project Overview

| 🧩 **Component** | 📋 **Description** |
|------------------|--------------------|
| ☁️ **Platform** | AWS (EC2) |
| 🪟 **OS** | Windows Server 2019 |
| 🔧 **Services** | Active Directory Domain Services, ServiceNow Developer |
| 🎯 **Goal** | Simulate daily helpdesk operations in a lab setting |

---

## ⚙️ EC2 Instance Setup

1. 🚀 Launched a **Windows Server 2019 EC2 instance** via AWS Console  
2. 🔐 Enabled **RDP access** through security groups (port `3389`)  
3. 🛠️ Chose **Role-Based** installation type  
4. 📥 Installed the **Active Directory Domain Services (AD DS)** role  
5. 🏰 Promoted the instance to a **Domain Controller** and created domain: `corp.local`  

---

## 👥 Active Directory | Create Users

1. 🔎 Search for **"Active Directory Users and Computers"**  
2. 📂 Expand the `corp.local` domain → go to **Users**  
3. ➕ Right-click → **New** → **User**  
4. 👤 Enter details + set a **secure password**

---

## 🧑‍🤝‍🧑 Active Directory | Create Groups

1. 🔎 Search for **"Active Directory Users and Computers"**  
2. 📂 Under `corp.local`, go to **Users**, right-click → **New** → **Group**  
3. 🧱 Name your group and set scope/type

---

## 🔐 Active Directory | Reset User Password

1. 🔎 Search for **"Active Directory Users and Computers"**  
2. 📂 Navigate to **Users**, right-click a user  
3. 🔄 Select **Reset Password**, enter a new secure password 🔑

---

## 🧩 Active Directory | Add User to Group

1. 🔎 Open **"Active Directory Users and Computers"**  
2. 📂 Find your group → Right-click → **Properties**  
3. ➕ Go to **Members** → Click **Add** → Enter username → Click **Apply** and **OK**

---

## 🔁 Lab Flow Diagram (Mermaid)

```mermaid
graph TD
    A[Launch EC2 Instance] --> B[Enable RDP Port 3389]
    B --> C[Install AD DS Role]
    C --> D[Promote to Domain Controller]
    D --> E[Create Domain: corp.local]
    E --> F[Create Users]
    F --> G[Create Groups]
    G --> H[Reset User Passwords]
    H --> I[Add Users to Groups]
