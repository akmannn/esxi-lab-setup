# ESXi Lab Setup

This repo documents my VMware ESXi 8 lab installation, VM configuration, networking, and troubleshooting notes.

## Overview
- **Host:** i7 10700 / 32GB / 954 GB SSD / RTX 2070 8GB (a bit overkill/irrelevant)
- **ESXi version:** ESXi 8.0U3e
- **Purpose:** Test VMs, learn virtualization, practice networking and backups.

## Installation steps
1. Create a bootable USB with the ESXi ISO and boot the host.
2. Follow the installer prompts:
   - Select target disk
   - Set root password
3. Configure management network (IP, gateway, DNS).

## VM Configuration
- VM1: `Windows-Server-2022` — CPU 2, RAM 4GB, Disk 60GB — role: Active Directory
- VM2: `Ubuntu-Server-22.04` — CPU 1, RAM 2GB, Disk 20GB — role: utility

## Networking
- vSwitch0: Management network
- vSwitch1: VM network (VLAN 10)
- Note any VLAN/trunk configs you used on your physical switch.

## Useful commands & notes
- **Enable SSH:** Host → Services → Enable SSH
- **CLI example (ESXi shell):**
```bash
# view network adapters
esxcli network nic list

# view datastore
esxcli storage filesystem list
