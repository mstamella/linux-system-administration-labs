# RHEL Repository Management

## Overview

This project demonstrates enterprise Linux software repository management on a **Red Hat Enterprise Linux 9** system.

Administrators often configure local and remote repositories to control software deployment, maintain package consistency, and support systems operating in restricted or offline environments.

This project aligns with **RHCSA (EX200)** objectives for software management and repository configuration.

---

## Lab Architecture

This lab simulates repository management for enterprise Linux systems.

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
| Package Manager | DNF |
| Repository Type | Local ISO Repository |
| Additional Source | Red Hat CDN |

---

## Objectives

- Configure local software repositories
- Manage repository configuration files
- Enable and disable repositories
- Verify repository availability
- Install software from configured repositories

---

## Implementation

### Local Repository Configuration

- Mounted RHEL installation ISO
- Created local repository directory
- Configured repository configuration file

### Repository Management

- Enabled repository configuration
- Verified repository availability
- Listed available repositories

### Software Installation

- Installed packages using configured repository
- Verified successful package installation

---

## Skills Demonstrated

- Linux package management
- Repository configuration
- Enterprise software deployment control
- Offline repository management
- Enterprise Linux system administration

---

## Commands Used

```bash
mount /dev/cdrom /repo
dnf config-manager --add-repo
dnf repolist
dnf install httpd
```

---

## Validation

Configuration was verified using:

```bash
dnf repolist
dnf list installed
```

---

## Outcome

Successfully configured enterprise Linux software repositories with:

- local ISO repository configuration
- repository management using DNF
- software installation from configured repositories
- verification of repository availability

---

## Summary

This project demonstrates enterprise Linux repository management including repository configuration, package installation, and software deployment using the DNF package manager.
