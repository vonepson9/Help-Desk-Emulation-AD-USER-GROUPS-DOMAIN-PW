#  Active Directory Helpdesk Lab on AWS EC2  
> Simulating real-world helpdesk ops in a cloud-hosted lab  
> 🖥 Powered by AWS EC2 |  Built with Active Directory

![OS](https://img.shields.io/badge/Windows_Server_2022-blue?logo=windows&logoColor=white)
![VM](https://img.shields.io/badge/Windows_10_Pro-blue?logo=windows&logoColor=white)
![Platform](https://img.shields.io/badge/AWS_EC2-FF9900?logo=amazon-aws&logoColor=white)
![Tools](https://img.shields.io/badge/PDQ_Deploy-lightgrey?logo=windows&logoColor=white)
![Tools](https://img.shields.io/badge/Active_Directory-003366?logo=microsoft&logoColor=white)

---

##  Lab Video Walkthroughs

- 🔹 [**Initial AD Setup + Users/Groups Demo (Loom)**](https://www.loom.com/share/ed8bf3cadec144938b287bedfa54f0ab?sid=5e67221e-bc8e-423a-bb85-1874cc0767ee)  
- 🔹 [**Expanded Features: Desktop Join, Shared Drives, PDQ (Google Drive)**](https://drive.google.com/file/d/1KpRvhTHnqaIia60Vi19vyY7RO-kJQVvL/view?usp=sharing)

---

##  Project Overview

|  **Component** |  **Description** |
|------------------|--------------------|
|  **Platform** | AWS (EC2) |
|  **OS** | Windows Server 2022 (DC), Windows 10 Pro (VM) |
|  **Services** | Active Directory Domain Services |
|  **Goal** | Simulate daily helpdesk operations in a lab setting |

---

##  EC2 Instance Setup

1.  Launched a **Windows Server 2022 EC2 instance** via AWS Console  
2.  Enabled **RDP access** through security groups (port `3389`)  
3.  Chose **Role-Based** installation type  
4.  Installed the **Active Directory Domain Services (AD DS)** role  
5.  Promoted the instance to a **Domain Controller** and created domain: `corp.local`  

---

##  Active Directory | Create Users

1.  Search for **"Active Directory Users and Computers"**  
2.  Expand the `corp.local` domain → go to **Users**  
3.  Right-click → **New** → **User**  
4.  Enter details + set a **secure password**

---

##  Active Directory | Create Groups

1.  Search for **"Active Directory Users and Computers"**  
2.  Under `corp.local`, go to **Users**, right-click → **New** → **Group**  
3.  Name your group and set scope/type

---

##  Active Directory | Reset User Password

1.  Search for **"Active Directory Users and Computers"**  
2.  Navigate to **Users**, right-click a user  
3.  Select **Reset Password**, enter a new secure password 🔑

---

##  Active Directory | Add User to Group

1.  Open **"Active Directory Users and Computers"**  
2.  Find your group → Right-click → **Properties**  
3.  Go to **Members** → Click **Add** → Enter username → Click **Apply** and **OK**

---

##  Expanded Lab Features | Desktop Join, Shared Drives & PDQ Deploy

-  Added a **Windows 10 Pro VM** to the `corp.local` domain to simulate real-world workstation integration  
-  Mapped **network drives** and configured **shared folders** for seamless domain-wide file access  
-  Deployed software to multiple machines using **PDQ Deploy**  
-  Showcased centralized IT management and automation best practices  

---

##  Lab Flow Diagram (Mermaid)

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
    I --> J[Add Desktop to Domain]
    J --> K[Map Shared Network Drives]
    K --> L[Deploy Software with PDQ]

