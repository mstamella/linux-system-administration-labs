# Enterprise Linux Server Deployment

## Overview
This lab demonstrates the deployment, configuration, and recovery of a **Red Hat Enterprise Linux 9 server** in a virtualized environment.

The system is configured to operate without external repositories and supports secure user management, system recovery, and persistent logging.

This project aligns with **RHCSA (EX200)** objectives for system installation, boot management, repositories, and administration.

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

## Tasks Performed

### Server Installation
- Installed **RHEL 9** using default partitioning
- Configured server installation profile
- Verified system boot targets and kernel parameters

### Repository Configuration
- Mounted installation ISO to `/repo`
- Configured local repository
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
## Outcome

Successfully deployed and configured an enterprise Linux server with:

- repository management using local and CDN repositories  
- secure authentication and password recovery procedures  
- system recovery through emergency boot mode  
- persistent system logging with journald  
---
### Summary

These tasks demonstrate core RHCSA system administration skills used in enterprise Linux environments including system recovery, repository management, and service administration.
