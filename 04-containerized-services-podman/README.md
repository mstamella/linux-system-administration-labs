
# Containerized Services with Podman

## Overview

This project demonstrates container deployment and management using **Podman** on a Red Hat Enterprise Linux 9 system.

The lab focuses on running containerized services, configuring container networking, and managing container lifecycles without requiring a daemon-based container engine.

This project aligns with **RHCSA (EX200)** objectives for container management and service deployment.

---

## Lab Architecture

This lab simulates deploying containerized services on an enterprise Linux server.

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
| Container Engine | Podman |
| Container Image | `nginx` |
| Network | Default Podman bridge |

---

## Objectives

- Install and configure Podman
- Pull container images from a registry
- Deploy containerized services
- Configure container port mappings
- Manage container lifecycle operations

---

## Implementation

### Podman Installation

- Verified Podman installation
- Confirmed container runtime functionality

### Image Management

- Pulled container images from a container registry
- Verified image availability

### Container Deployment

- Deployed an **`nginx` web server container**
- Configured container port mapping
- Verified container service accessibility

### Container Management

- Started and stopped containers
- Inspected container configuration
- Removed unused containers and images

---

## Skills Demonstrated

- Container runtime management using Podman
- Container image management
- Containerized web service deployment
- Container networking and port mapping
- Container lifecycle management

---

## Commands Used

```bash
podman version
podman pull nginx
podman images
podman run -d --name webserver -p 8080:80 nginx
podman ps
podman stop <container_id>
podman rm <container_id>
podman rmi nginx
```
---

## Validation

Configuration was verified using:

```bash
podman ps
podman images
curl http://localhost:8080
```
---

## Outcome

Successfully deployed a containerized web service using Podman with:

- container image retrieval from a registry
- containerized `nginx` webserver deployment
- container networking with port mapping
- container lifecycle management using Podman commands

---

## Summary

This project demonstrates container deployment and management on enterprise Linux systems using Podman, including container runtime operation, service deployment, and container lifecycle management.

