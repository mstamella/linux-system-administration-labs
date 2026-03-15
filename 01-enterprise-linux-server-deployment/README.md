# Enterprise Linux Server Deployment

## Overview
This project demonstrates the deployment, configuration, and recovery of a **Red Hat Enterprise Linux 9 server** in a virtualized environment.

The system is configured to operate without external repositories and supports secure user management, system recovery, and persistent logging.

This project aligns with **RHCSA (EX200)** objectives for system installation, boot management, repositories, and administration.

---

## Lab Architecture

This lab simulates an enterprise Linux server deployment environment.

**Host System**
- macOS or Windows workstation

**Virtualization Platform**
- VirtualBox

**Guest Operating System**
- Red Hat Enterprise Linux 9

**Resources**
- 2 GB RAM  
- 20 GB primary disk  
- Additional disk used for storage labs

---

## Lab Environment

| Component | Configuration |
|----------|---------------|
| OS | RHEL 9 |
| Platform | VirtualBox |
| RAM | 2 GB |
| Disk | 20 GB primary disk |
| Additional Storage | Secondary disk for storage labs |

---

## Objectives

- Deploy a Red Hat Enterprise Linux server
- Configure local software repositories
- Practice system recovery procedures
- Configure system logging and boot targets
- Validate system configuration

---

## Implementation

### Server Installation
- Installed **RHEL 9** using default partitioning
- Configured server installation profile
- Verified system boot targets and kernel parameters

### Repository Configuration
- Mounted installation ISO to `/repo`
- Configured a local software repository
- Disabled external repositories

### System Recovery
- Booted into **emergency mode**
- Reset lost root password
- Verified system integrity after reboot

### System Configuration
- Configured system logging using `journald`
- Installed software from local repositories
- Registered system using `subscription-manager`
- Enabled **Red Hat CDN repositories**

---

## Skills Demonstrated

- Linux server deployment
- Boot troubleshooting and system recovery
- Repository configuration
- System logging and service management
- Enterprise Linux administration

---

## Commands Used

```bash
mount /dev/cdrom /repo
dnf config-manager --add-repo
systemctl set-default multi-user.target
passwd root
journalctl -xe
```
---

## Validation

Configuration was verified using:

```bash
systemctl get-default
dnf repolist
journalctl -xe
```

### Outcome
• repository management  
• authentication and recovery  
• emergency boot recovery  
• journald logging  

### Summary

### Outcome
• repository management  
• authentication and recovery  
• emergency boot recovery  
• journald logging  

### Summary

This project demonstrates core RHCSA system administration skills used in enterprise Linux environments including system recovery, repository management, and service administration.

---


