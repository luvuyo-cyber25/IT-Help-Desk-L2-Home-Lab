# IT Helpdesk Level 2 Lab – Windows Server, Active Directory & Enterprise Support

**Project Overview**  
This comprehensive lab simulates a full Level 2 IT Helpdesk / Junior Systems Administrator role in a corporate environment. Built entirely in VirtualBox, I deployed a Windows Server 2016 Domain Controller, configured Active Directory from scratch, managed users/groups/OUs/policies, set up file shares/printers, joined client workstations, implemented security controls, performed remote troubleshooting, deployed software with PDQ tools, worked with ticketing systems, and applied delegation of control. 

The lab progresses logically from basic server setup through advanced administration, security, remote support, and automation. 

**Features**  
- Complete Windows domain deployment (Server 2016 → Domain Controller with `kevtech.com` / `kevcaftec.com`)  
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
