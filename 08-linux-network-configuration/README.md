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

- Identified active network interface using nmcli before applying configuration changes
- Listed available network interfaces
- Verified active network connections
- Confirmed network device status

### Network Configuration

- Configured network interface using persistent NetworkManager connection profiles via nmcli  
- Modified connection settings including IPv4 method, IP address, gateway, and DNS parameters  
- Applied configuration changes by bringing the connection up using nmcli  

### Connectivity Verification

- Verified network configuration changes were successfully applied and active  
- Tested connectivity between hosts using ping  

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
nmcli connection modify <connection-name> ipv4.method auto
nmcli connection up <connection-name>
ip addr
ping -c 2 rhcsa4
```

---

## Validation

Verified network configuration and connectivity:

```bash
nmcli device status         # Confirmed active interface and connection state
ip addr                     # Verified IP address assignment
ping -c 2 rhcsa3            # Verified connectivity from peer host
ping -c 2 rhcsa4            # Verified connectivity to peer host
```

---

## Outcome

Successfully configured and validated Linux network connectivity using NetworkManager, including interface configuration, connection management, and connectivity verification, with configurations tested for persistence and reliability.

Key outcomes:

- Network interface inspection and validation  
- Network configuration using nmcli  
- Verification of active network connections  
- Successful host-to-host connectivity testing  
- Troubleshooting using system-level diagnostic commands  


---

## Summary

This project demonstrates enterprise Linux network configuration including interface management, network verification, and connectivity testing using NetworkManager and nmcli.
