# Enterprise Linux System Administration Lab Portfolio

Hands-on **Linux system administration projects** aligned with **Red Hat Certified System Administrator (RHCSA EX200)** objectives.

This repository demonstrates practical experience administering **Red Hat Enterprise Linux 9** systems including server deployment, storage management, user security, containerized services, application management, repository configuration, networking, and system automation.

All projects were performed in a controlled lab environment using enterprise Linux administration tools and documented using real commands and validation steps.

The projects in this repository simulate common enterprise Linux administration tasks performed by system administrators in production environments.

---

# Lab Environment

| Component | Configuration |
|----------|---------------|
| Host System | macOS / Windows |
| Virtualization | VirtualBox |
| Guest OS | Red Hat Enterprise Linux 9 |
| RAM | 2 GB |
| Storage | 20 GB + additional disks |
| Networking | VirtualBox NAT |

---

## Project Index

| Project | Topic | Key Skills |
|-------|------|------|
| [01 Enterprise Linux Server Deployment](https://github.com/mstamella/linux-system-administration-labs/tree/main/01-enterprise-linux-server-deployment) | Server installation | RHEL install, boot recovery, journald |
| [02 Storage Management with GPT & LVM](https://github.com/mstamella/linux-system-administration-labs/tree/main/02-storage-management-lvm-gpt) | Storage administration | GPT partitioning, LVM, filesystem expansion |
| [03 Secure Multi-User Linux Environment](https://github.com/mstamella/linux-system-administration-labs/tree/main/03-secure-multi-user-linux-environment) | User security | Users, groups, ACLs, sudo |
| [04 Containerized Services with Podman](https://github.com/mstamella/linux-system-administration-labs/tree/main/04-containerized-services-podman) | Containers | Podman, container networking |
| [05 Linux Automation with systemd Timers](https://github.com/mstamella/linux-system-administration-labs/tree/main/05-linux-automation-systemd-timers) | Automation | systemd services, timers |
| [06 Flatpak Application Management](https://github.com/mstamella/linux-system-administration-labs/tree/main/06-flatpak-application-management) | Application management | Flatpak, Flathub repositories |
| [07 RHEL Repository Management](https://github.com/mstamella/linux-system-administration-labs/tree/main/07-rhel-repository-management) | Software repositories | DNF, local ISO repos |
| [08 Linux Network Configuration](https://github.com/mstamella/linux-system-administration-labs/tree/main/08-linux-network-configuration) | Networking | nmcli, interface configuration |

---

# Projects

## 1. Enterprise Linux Server Deployment

Deployment and configuration of a Red Hat Enterprise Linux server including system recovery, boot management, and repository configuration.

**Skills demonstrated**

- RHEL installation and configuration
- repository management
- boot troubleshooting
- system recovery
- system logging using journald

📁 [01-enterprise-linux-server-deployment](https://github.com/mstamella/linux-system-administration-labs/tree/main/01-enterprise-linux-server-deployment)

---

## 2. Storage Management with GPT and LVM

Enterprise Linux storage configuration using GPT partitioning, Logical Volume Manager (LVM), and online filesystem expansion.

**Skills demonstrated**

- GPT disk partitioning
- physical volume initialization
- volume group management
- logical volume creation
- filesystem resizing
- persistent mounts using `/etc/fstab`

📁 [02-storage-management-lvm-gpt](https://github.com/mstamella/linux-system-administration-labs/tree/main/02-storage-management-lvm-gpt)

---

## 3. Secure Multi-User Linux Environment

Secure multi-user system configuration including user management, group permissions, Access Control Lists (ACLs), and controlled privilege escalation.

**Skills demonstrated**

- user administration
- group management
- file permissions and ownership
- ACL configuration
- shared directory access control
- sudo privilege management

📁 [03-secure-multi-user-linux-environment](https://github.com/mstamella/linux-system-administration-labs/tree/main/03-secure-multi-user-linux-environment)

---

## 4. Containerized Services with Podman

Deployment and management of containerized services using the Podman container engine.

**Skills demonstrated**

- container runtime management
- container image management
- containerized web server deployment
- container networking
- container lifecycle management

📁 [04-containerized-services-podman](https://github.com/mstamella/linux-system-administration-labs/tree/main/04-containerized-services-podman)

---

## 5. Linux Automation with systemd Timers

Automation of administrative tasks using systemd service units and systemd timers.

**Skills demonstrated**

- systemd service configuration
- systemd timer scheduling
- automated task execution
- service lifecycle management

📁 [05-linux-automation-systemd-timers](https://github.com/mstamella/linux-system-administration-labs/tree/main/05-linux-automation-systemd-timers)

---

## 6. Flatpak Application Management

Application deployment and management using Flatpak package management.

**Skills demonstrated**

- Flatpak installation
- repository configuration using Flathub
- secure application deployment
- Flatpak application lifecycle management

📁 [06-flatpak-application-management](https://github.com/mstamella/linux-system-administration-labs/tree/main/06-flatpak-application-management)

---

## 7. RHEL Repository Management

Enterprise Linux repository configuration including local ISO repositories and package installation using DNF.

**Skills demonstrated**

- repository configuration
- local repository management
- package installation using DNF
- repository verification

📁 [07-rhel-repository-management](https://github.com/mstamella/linux-system-administration-labs/tree/main/07-rhel-repository-management)

---

## 8. Linux Network Configuration

Network configuration and connectivity verification using NetworkManager and `nmcli`.

**Skills demonstrated**

- network interface management
- NetworkManager administration
- network configuration using nmcli
- connectivity verification

📁 [08-linux-network-configuration](https://github.com/mstamella/linux-system-administration-labs/tree/main/08-linux-network-configuration)

---

# Core Skills Demonstrated

- Red Hat Enterprise Linux administration
- Linux system deployment
- storage management (GPT, LVM)
- multi-user security and permissions
- container management with Podman
- Linux automation using systemd
- software and repository management
- Linux network configuration

---

# Author

Tammie Freeman  
Junior Linux System Administrator  
Master of Engineering (M.Eng.), Cybersecurity Policy & Compliance  
CompTIA Linux+ | CompTIA Security+ | RHCSA (In Progress)
