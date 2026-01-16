# IT Helpdesk Level 2 Lab – Windows Server, Active Directory & Enterprise Support

**Project Overview**  
This comprehensive lab simulates a full Level 2 IT Helpdesk / Junior Systems Administrator role in a corporate environment. Built entirely in VirtualBox, I deployed a Windows Server 2016 Domain Controller, configured Active Directory from scratch, managed users/groups/OUs/policies, set up file shares/printers, joined client workstations, implemented security controls, performed remote troubleshooting, deployed software with PDQ tools, worked with ticketing systems, and applied delegation of control. 

The lab progresses logically from basic server setup through advanced administration, security, remote support, and automation. 

**Features**  
- Complete Windows domain deployment (Server 2016 → Domain Controller with `VUYOTECH.COM`)  
- Active Directory management: OUs, users, groups, delegation of control, recycle bin  
- Group Policy: Password/lockout policies, restrictions (e.g., disable Task Manager)  
- File server: Departmental shares + automated home drives with group-based NTFS permissions  
- Printer management: Print Server role, AD-published printers, group permissions  
- Client management: Domain join, RSAT tools, static IPs, Host-only networking  
- Remote support: RDP, Quick Assist, admin shares, Remote Registry, Zoho-style sessions  
- Troubleshooting: Account lockouts/unlocks, password resets, gpresult, net use, Account Lockout Status tool  
- Software & inventory: PDQ Deploy (silent installs), PDQ Inventory (hardware/software reporting)  
- Ticketing & ITSM: Spiceworks help desk workflow demonstration  
- Security best practices: Least privilege, inheritance disabling, enforced policies

## Screenshots

### Active Directory Domain Overview
![Active Directory Domain Overview](Active%20Directory%20Domain%20Overview.png)  
![Active Directory Domain Overview Alt 1](Active%20Directory%20Domain%20Overview%20Alt%201.png)  
Shows the full domain structure with OUs, users, and groups.

### Group Policy Configuration
![Group Policy Account Lockout](Group%20Policy%20Account%20Lockout.png)  
![Group Policy User Restrictions](Group%20Policy%20User%20Restrictions.png)  
Displays account lockout policy (6 attempts, 30 min) and user restrictions (e.g., disabled Task Manager).

### OU Design and Delegation
![OU Design](OU%20Design.png)  
Shows organizational units, delegation of control, and password reset permissions.

### Network Drive Mapping
![Network Drive Mapping](Network%20Drive%20Mapping.png)  
Mapped departmental drives (HR, Personal) and home directories with proper NTFS permissions.

### Print Server Configuration
![Print Server Permissions](Print%20Server%20Permissions.png)  
![Print Server Overview](Print%20Server%20Overview.png)  
Demonstrates print server setup and group-based access control for printers.

### Client Domain Join
![Client Domain Join](Client%20Domain%20Join.png)  
![Client Domain Join Alt 1](Client%20Domain%20Join%20Alt%201.png)  
Evidence of clients successfully joining the domain and appearing in ADUC.

### Remote Desktop Support
![Remote Desktop RDP Session](Remote%20Desktop%20RDP%20Session.png)  
![Remote Desktop RDP Session Alt 1](Remote%20Desktop%20RDP%20Session%20Alt%201.png)  
Shows remote support session via RDP with administrative access.

### PDQ Deploy Software Deployment
![PDQ Deploy Software Deployment](PDQ%20Deploy%20Software%20Deployment.png)  
Demonstrates silent software deployment (e.g., Zoom) to domain clients.

### PDQ Inventory – Asset Management
![PDQ Inventory System Details](PDQ%20Inventory%20System%20Details.png)  
![PDQ Inventory Hardware Software Report](PDQ%20Inventory%20Hardware%20Software%20Report.png)  
Shows hardware/software inventory, updates, and reports for endpoint management.

### IT Support & Ticketing
![Spiceworks Ticketing Workflow](Spiceworks%20Ticketing%20Workflow.png)  
![IT Support Troubleshooting](IT%20Support%20Troubleshooting.png)  
Highlights ticketing workflow, account lockout troubleshooting, and remote session handling.



**Installation & Lab Build Steps** (High-Level Summary)  
1. Installed VirtualBox → created isolated Host-only network  
2. Deployed Windows Server 2016 Datacenter → static IP → promoted to Domain Controller  
3. Configured AD: OUs, users (helpdesk, Patty, Scott), security groups, delegation (password reset only)  
4. Applied Group Policies: Lockout (4 attempts), password age (90 days), restrictions (disable Task Manager)  
5. Created Windows 10 Pro clients → RSAT tools → domain join  
6. Set up file shares (HR, Personal) + home drives (%username%) with least-privilege NTFS  
7. Installed Print Server role → shared/published printer → group permissions  
8. Performed remote support: RDP, Quick Assist, admin shares, Remote Registry  
9. Deployed software silently with PDQ Deploy (e.g., Zoom)  
10. Used PDQ Inventory: Hardware/software inventory, reports, remote actions (restart, MMC)  
11. Demonstrated ticketing workflow in Spiceworks + remote session (Zoho-style)  
12. Troubleshot: Lockouts (Account Lockout Status tool), resets, gpupdate / gpresult  

**Technologies & Skills Gained**

**Tools & Technologies**  
- VirtualBox  
- RSAT tools  
- Account Lockout Status Tool  
- RDP  
- PDQ  
- Spiceworks  
- Windows Server 2016  
- Active Directory Domain Services (AD DS)  
- Active Directory Users and Computers (ADUC)  
- Group Policy Management Console (GPMC)  
- Command Prompt (CMD)  
- Print Management Console  
- Server Manager  

**Skills Gained**  
- Virtualization  
- Server Administration  
- Active Directory  
- Network Configuration  
- Ticketing System  
- Group Policy Management  
- DNS  
- Network Drive Mapping  
- TCP/IP  
- User Account Lifecycle Management  
- Organizational Unit (OU) Design  
- NTFS & Share Permissions Configuration  
- Remote Desktop & Support  
- Account Lockout Troubleshooting  
- Software Deployment  

This lab demonstrates end-to-end ownership of a Windows domain environment, making it highly relevant for **IT Helpdesk L2**, **Desktop Support**, **Junior SysAdmin**, and **Systems Engineer** roles.
