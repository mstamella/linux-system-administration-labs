# Storage Management with GPT and LVM

## Overview

This project demonstrates enterprise Linux storage administration using **GPT partitioning, Logical Volume Manager (LVM), and filesystem resizing**.

The lab simulates real-world Linux system administration tasks where additional disks are provisioned and storage must be dynamically expanded without downtime.

This project aligns with **RHCSA (EX200)** objectives for disk partitioning, logical volume management, filesystem creation, and storage expansion.

---

## Lab Architecture

This lab simulates adding new storage to a running Linux server.

**Host System**
- macOS or Windows workstation

**Virtualization Platform**
- VirtualBox

**Guest Operating System**
- Red Hat Enterprise Linux 9

**Resources**

- 2 GB RAM
- 20 GB primary disk
- additional disk for storage configuration

---

## Lab Environment

| Component | Configuration |
|----------|---------------|
| OS | RHEL 9 |
| Platform | VirtualBox |
| RAM | 2 GB |
| Primary Disk | 20 GB |
| Additional Disk | Storage configuration |

---

## Objectives

- Create **GPT partition tables**
- Initialize **physical volumes**
- Create **volume groups**
- Create and manage **logical volumes**
- Expand logical volumes and filesystems
- Configure **persistent mounts**

---

## Implementation

### Disk Partitioning

- Created **GPT partition table**
- Added partition for LVM usage
- Verified disk layout

### LVM Configuration

- Initialized **physical volume**
- Created **volume group**
- Created **logical volume**

### Filesystem Configuration

- Created **XFS filesystem**
- Mounted logical volume
- Configured persistent mount configuration using `/etc/fstab`

### Storage Expansion

- Extended logical volume
- Resized filesystem online without downtime

---

## Skills Demonstrated

- GPT disk partitioning
- LVM storage architecture
- Filesystem creation and management
- Online storage expansion
- Persistent filesystem mounts
- Enterprise Linux storage administration

---

## Commands Used

```bash
lsblk
parted /dev/sdb
pvcreate /dev/sdb1
vgcreate data_vg /dev/sdb1
lvcreate -L 5G -n data_lv data_vg
mkfs.xfs /dev/data_vg/data_lv
mount /dev/data_vg/data_lv /data
lvextend -L +2G /dev/data_vg/data_lv
xfs_growfs /data
```
---

## Validation

Configuration was verified using:

```bash
lsblk
pvs
vgs
lvs
df -h
mount
```
---

## Outcome

Successfully configured enterprise Linux storage with:

- GPT partitioning for modern disk management
- Logical volume management using LVM
- XFS filesystem creation and mounting
- Online logical volume expansion
- Persistent mount configuration using /etc/fstab

---

## Summary

This project demonstrates enterprise Linux storage administration including disk partitioning, LVM configuration, filesystem management, and online storage expansion.
