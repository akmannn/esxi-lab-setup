# ESXi Lab Setup

A fully documented virtualization & systems administration lab running on VMware ESXi 8.0.3, showcasing:

- **ISO creation (Windows Server & Windows 10/11)**
- **ESXi deployment on bare metal**
- **Active Directory Domain Services**
- **DHCP, DNS, GPO**
- **Domain-joined Windows clients**
- **Network design, static/DHCP addressing**
- **Troubleshooting logs**
- **Configuration notes**

This project demonstrates real-world **systems administration, virtualization, and enterprise IT** skills.

## 🔧 Lab Overview
| Component         | Hostname             | IP Address                 | Purpose                   |
| ----------------- | -------------------- | -------------------------- | ------------------------- |
| ESXi Host         | esxi01.home          | **192.168.2.201**          | Hypervisor (bare metal)   |
| Domain Controller | **DC01.akman.local** | **192.168.2.202** (static) | AD DS, DNS, DHCP          |
| Windows Client    | **WC01.akman.local** | **192.168.2.233** (DHCP)   | Domain-joined workstation |
| DHCP Scope        | Akman_scope          | 192.168.2.231–240          | Addressing for clients    |

This repo documents my VMware ESXi 8 lab installation, VM configuration, networking, and troubleshooting notes.

📂 Repository Sections
| Folder                       | Description                                         |
| ---------------------------- | --------------------------------------------------- |
| **01-iso-creation**          | ISO creation process using PowerShell + screenshots |
| **02-esxi-installation**     | Bare-metal ESXi installation screenshots            |
| **03-dc01-setup**            | Windows Server 2019 → AD DS → DNS → Domain config   |
| **04-wc01-setup**            | Windows client installation + domain join           |
| **05-network-configuration** | vSwitch0, vmk0, NIC mapping, VLANs                  |
| **06-dhcp-configuration**    | DHCP scope, reservations, bindings                  |

Each section has its own README with step-by-step guides and screenshots.


