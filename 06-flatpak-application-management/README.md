# Flatpak Application Management

## Overview

This project demonstrates application management using **Flatpak** on a Red Hat Enterprise Linux 9 system.

Flatpak provides a secure and isolated method of installing and managing applications independent of the base operating system. This allows administrators to deploy software in a controlled environment without affecting core system packages.

This project aligns with **RHCSA (EX200)** objectives related to software management and repository configuration.

---

## Lab Architecture

This lab simulates enterprise application deployment using Flatpak package management.

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
| Package Manager | Flatpak |
| Repository | Flathub |
| Application | Sample Flatpak application |

---

## Objectives

- Install Flatpak package management
- Configure Flatpak repositories
- Install applications using Flatpak
- Manage installed Flatpak applications
- Verify application deployment

---

## Implementation

### Flatpak Installation

- Installed Flatpak package manager
- Verified Flatpak installation

### Repository Configuration

- Added the **Flathub** Flatpak repository
- Verified repository configuration

### Application Installation

- Installed application from Flatpak repository
- Verified application installation

### Application Management

- Listed installed Flatpak applications
- Verified application availability

---

## Skills Demonstrated

- Linux software management
- Flatpak application deployment
- Repository configuration
- Secure application installation
- Application lifecycle management

---

## Commands Used

```bash
dnf install flatpak
flatpak remote-add --if-not-exists flathub https://flathub.org/repo/flathub.flatpakrepo
flatpak install flathub <application>
flatpak list
flatpak run <application>
```

---

## Validation

```bash
flatpak list
flatpak remotes
```

---

## Outcome

Successfully implemented application deployment using Flatpak with:

- Flatpak package management installation
- Fepository configuration using Flathub
- application installation from Flatpak repository
- verification of installed Flatpak applications

---

## Summary

This project demonstrates enterprise Linux application management using Flatpak including repository configuration, secure application deployment, and Flatpak package lifecycle management.

