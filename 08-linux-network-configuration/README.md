# Linux Network Configuration

## Overview

This project demonstrates network configuration and management on a **Red Hat Enterprise Linux 9** system using NetworkManager and the `nmcli` command-line interface.

Administrators frequently configure network interfaces, assign IP addresses, and verify network connectivity to ensure systems communicate reliably within enterprise environments.

This project aligns with **RHCSA (EX200)** objectives for network configuration and connectivity verification.

---

## Lab Architecture

This lab simulates configuring network interfaces on an enterprise Linux server.

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
| Network Manager | NetworkManager |
| Interface Tool | nmcli |
| Network Mode | VirtualBox NAT |

---

## Objectives

- View and manage network interfaces
- Configure network settings using nmcli
- Assign IP addressing information
- Enable and disable network connections
- Verify network connectivity

---

## Implementation

### Network Interface Inspection

- Listed available network interfaces
- Verified active network connections
- Confirmed network device status

### Network Configuration

- Used **nmcli** to configure network settings
- Verified interface configuration
- Restarted network connections when necessary

### Connectivity Verification

- Tested network connectivity
- Verified system network access
- Confirmed network configuration changes

---

## Skills Demonstrated

- Linux network interface management
- NetworkManager administration
- Network configuration using nmcli
- Network troubleshooting
- Connectivity verification

---

## Commands Used

```bash
nmcli device status
nmcli connection show
nmcli connection up
ip addr
ping google.com
```

---

## Validation

```bash
nmcli device status
ip addr
ping google.com
```

---

## Outcome

Succesfully configured and verified Linux network connectivity using NetworkManager with:

- network interface inspection
- network configuration using nmcli
- verification of active network connection
- successful connectivity testing

---

## Summary

This project demonstrates enterprise Linux network configuration including interface management, network verification, and connectivity testing using NetworkManager and nmcli.
