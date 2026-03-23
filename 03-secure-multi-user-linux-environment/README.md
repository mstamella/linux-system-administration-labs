# Secure Multi-User Linux Environment

## Overview

This project demonstrates secure multi-user administration on a **Red Hat Enterprise Linux 9** system.

The lab focuses on user account management, group administration, file permissions, access control lists (ACLs), and controlled privilege escalation using sudo.

This project aligns with **RHCSA (EX200)** objectives for user and group management, permission management, and secure system access.

---

## Lab Architecture

This lab simulates a shared enterprise Linux environment where multiple users require controlled access to system resources.

**Host System**

- macOS or Windows workstation

**Virtualization Platform**

- VirtualBox

**Guest Operating System**

- Red Hat Enterprise Linux 9

---

## Lab Environment

| Component | Configuration |
|----------|---------------|
| OS | RHEL 9 |
| Platform | VirtualBox |
| User Accounts | Multiple test users |
| Shared Directory | `/shared` |
| Security Controls | Groups, permissions, ACLs, sudo |

---

## Objectives

- Create and manage user accounts
- Create and manage groups
- Configure secure shared directories
- Manage file permissions
- Configure Access Control Lists (ACLs)
- Configure controlled administrative access using sudo

---

## Implementation

### User and Group Management

- Created multiple user accounts
- Created administrative and shared access groups
- Assigned users to secondary groups

### Shared Directory Configuration

- Created a shared directory `/shared`
- Configured group ownership
- Set directory permissions to allow controlled collaboration

### Permission Management

- Configured standard Linux file permissions
- Applied group-based access control
- Verified permission inheritance

### Access Control Lists (ACLs)

- Applied ACLs to grant specific user access
- Verified ACL configuration

### Privilege Escalation

- Configured sudo access for administrative users
- Verified limited administrative command execution

---

## Skills Demonstrated

- Linux user administration
- Group management
- File permissions and ownership
- Access Control List (ACL) management
- Secure shared directory configuration
- Privilege escalation control using sudo

---

## Commands Used

```bash
useradd alice
useradd bob
groupadd devops
usermod -aG devops alice
mkdir /shared
chown :devops /shared
chmod 2770 /shared
setfacl -m u:bob:rwx /shared
getfacl /shared
visudo
```
---

## Validation

Configuration was verified using:

```bash
id alice
id bob
groups alice
ls -ld /shared
getfacl /shared
sudo -l
```

---

## Outcome

Successfully implemented a secure multi-user Linux environment with:
- controlled user and group management
- secure shared directory permissions
- extended permissions using ACLs
- controlled administrative access using `sudo`
- verification of user access and privilege boundaries

---

## Summary

This project demonstrates enterprise Linux user administration and access control including user management, group permissions, ACL configuration, and controlled privilege escalation.

