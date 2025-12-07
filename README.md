# IT Helpdesk Lab

## Project Overview
This lab simulates a real-world IT Helpdesk environment using Windows Server 2022, Active Directory Domain Services (AD DS), Group Policy Management, Windows 10/11 clients, file sharing, remote administration, and patch management. It demonstrates user management, domain configuration, network setup, endpoint onboarding, SMB permissions, and enterprise-style troubleshooting.

I built this lab to understand core Helpdesk/IT Support workflows such as domain joins, GPO enforcement, account management, remote access, and system updates.

## Features
Active Directory Setup

- Installed Windows Server 2022 and promoted it to a Domain Controller
- Created a new forest and domain: vuyotech.com
- Created AD users (e.g., Walter, Luvuyo) with proper account configurations
- Created AD groups (e.g., Tech) and assigned users

Domain & Network Configuration

- Configured VirtualBox networking (Host-Only, NAT, Bridged)
- Assigned static IPs for server and clients (10.x.x.x network)
- Joined Windows 10 machine to the vuyotech.com domain
- Verified connectivity using ping and DNS lookups

Group Policy Management

- Set password expiration (30 days)
- Configured account lockout threshold (3 attempts, 30-min lockout)
- Tested lockout behavior and account recovery
- Modified user logon hours and account expiration settings

Remote Administration

- Enabled Remote Desktop on the server
- Used Windows 10 machine to connect via RDP using domain credentials

SMB File Sharing & Permissions

- Created SMB share vuyotech on the server
- Created subfolders: Tech, HR, IT
- Applied NTFS & Share permissions:
- Removed “Everyone”
- Assigned the Tech group modify/read access
- Tested access from Windows 10 as user Walter
- Demonstrated that folder changes synced across clients (e.g., created “hack.txt”)

User & Computer Management

- Disabled/Enabled accounts
- Forced password resets
- Viewed user policies using net user /domain
- Managed account lockouts and restored user access

Patch & Endpoint Management

- Installed Action1 RMM agent
- Onboarded server and endpoints to Action1 console
- Deployed pending Windows updates remotely
- Tested deployment using both single-agent install and domain-wide deployer

Virtualization & System Administration

- Multi-VM setup on VirtualBox
- Used shared folders between host and server
- Installed Guest Additions and mounted shared resources
- Performed network reconfiguration across NAT/Bridged/Host-Only environments

Tools & Skills Gained
Technical Skills

Active Directory Administration: Users, groups, OUs, domain join

Group Policy Management: Security policies, password rules, lockout policy

Networking: DNS, static IPs, ping testing, TCP/IPv4 configuration

Remote Administration: RDP, domain authentication

File Sharing (SMB): NTFS permissions, share permissions, folder security

Patch Management: Action1 RMM deployment and update management

Troubleshooting: Account lockouts, login errors, permission issues

Virtualization: VirtualBox networking modes, VM provisioning

Windows Client Support: Windows 10/11 setup and domain integration
