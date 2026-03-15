# Linux Automation with systemd Timers

## Overview

This project demonstrates Linux system automation using **systemd services and systemd timers** on a Red Hat Enterprise Linux 9 system.

The lab focuses on automating administrative tasks using native systemd scheduling instead of traditional cron jobs.

This project aligns with **RHCSA (EX200)** objectives for service management, system automation, and timer-based task scheduling.

---

## Lab Architecture

This lab simulates automated system maintenance tasks on an enterprise Linux server.

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
| Automation Tool | systemd |
| Scheduled Task | File creation task |
| Timer Type | systemd timer unit |

---

## Objectives

- Create systemd service units
- Configure systemd timer units
- Automate administrative tasks
- Enable persistent automated execution
- Verify scheduled task execution

---

## Implementation

### Service Unit Creation

- Created a custom **systemd service unit**
- Configured service to run an automated administrative command

### Timer Unit Configuration

- Created a **systemd timer unit**
- Configured timer to execute the service on a scheduled interval

### Timer Management

- Enabled the timer unit
- Verified scheduled execution
- Confirmed automated task completion

---

## Skills Demonstrated

- systemd service configuration
- systemd timer scheduling
- Linux system automation
- service lifecycle management
- automated task validation

---

## Commands Used

```bash
systemctl daemon-reload
systemctl enable mytask.timer
systemctl start mytask.timer
systemctl list-timers
systemctl status mytask.timer
```
---

## Validation

```bash
systemctl list-timers
systemctl status mytask.timer
ls /tmp
```
---

## Outcome

Successfully implemented automated system administration tasks using systemd timers with:

- custom systemd service units
- scheduled execution using systemd timers
- automated task verification
- persistent timer configuration

---

## Summary

This project demonstrates Linux system automation using systemd services and timers to schedule administrative tasks in enterprise Linux environments.ls /tmp

