# Homelab Portfolio

This repository documents my personal homelab, which I built to gain hands-on experience with real-world IT systems and workflows. The lab is designed to reflect how small-to-mid-sized enterprise environments are actually deployed, managed, and maintained, using virtualization, Windows and Linux servers, centralized identity management, and containerized services.

The goal of this homelab isn’t just to spin things up, but to understand how systems are installed, verified, administered, and documented in a professional IT environment.

---

## Lab Purpose & Goals

I built this homelab to strengthen my system administration and cybersecurity skills by working through real configuration tasks instead of relying only on theory or guided labs. Everything in this environment is intentionally set up, tested, and validated to mirror how infrastructure is handled in production.

The main goals of this lab are to:
- Build and manage virtualized infrastructure using Proxmox VE
- Administer both Windows and Linux server operating systems
- Implement centralized identity and access management with Active Directory
- Practice role-based access control (RBAC) using users, groups, and OUs
- Deploy and validate containerized services using Docker
- Manage containers using Portainer for visibility and lifecycle control
- Verify configurations using command-line tools and PowerShell
- Document workflows in a way that reflects real operational practices

Overall, this lab emphasizes **installing services, verifying they work, and managing them over time**, which matches how systems are handled in real IT roles.

---

## Lab Implementation & Screenshots

### Proxmox Virtualization Host
![Proxmox Server](screenshots/proxmox-server.png)

Proxmox VE serves as the core platform for the homelab. It hosts and manages all virtual machines, providing centralized control, snapshots, and resource allocation across the environment.

---

### Windows Server Deployment
![Windows Server Installation](screenshots/windows-server-installation.png)

Windows Server deployed as a virtual machine within Proxmox. This system provides the foundation for enterprise identity services and Windows-based server administration tasks.

---

## Active Directory Domain Services (AD DS)

### AD DS Installation
![Active Directory Installation](screenshots/active-directory-role-installation.png)

Active Directory Domain Services installed on Windows Server using PowerShell to enable centralized authentication and identity management.

---

### AD Service Verification
![Active Directory NTDS Service Running](screenshots/active-directory-ntds-service-running.png)

The NTDS service verified as running through PowerShell, confirming that Active Directory was installed correctly and is functioning as expected.

---

### Domain Creation and Verification
![Active Directory Domain Details](screenshots/active-directory-domain-created.png)

The Windows Server was promoted to a domain controller, and a new Active Directory domain was created and validated using PowerShell.

---

### AD Object Management (Users, Groups, and OUs)
![Active Directory OUs](screenshots/active-directory-ou-structure.png)

Organizational Units were created to logically separate domain controllers and user accounts, reflecting how Active Directory is structured in real environments.

![Active Directory Groups](screenshots/active-directory-group-membership.png)

Security groups were created and managed using PowerShell, with users assigned to role-based groups to demonstrate RBAC and centralized permission management.

---

### Ubuntu Server Deployment
![Ubuntu Server Install](screenshots/Ubuntu%20Server%20Install.png)

Ubuntu Server LTS deployed as a virtual machine for Linux system administration, service hosting, and command-line management tasks.

---

### Ubuntu Static IP Configuration
![Ubuntu Static IP](screenshots/Ubuntu%20Server%20-%20Static%20IP%20Creation.png)

A static IP configuration applied to ensure consistent and predictable network access, similar to how servers are configured in production environments.

---

## Docker & Container Management

### Docker Installation Verification
![Docker Hello World](screenshots/docker-hello-world-test.png)

Docker installation verified using the official `hello-world` container to confirm proper client–daemon communication, image retrieval, and container execution.

---

### Portainer Deployment via Docker
![Portainer Install](screenshots/portainer-install-docker.png)

Portainer CE deployed as a Docker container on Ubuntu Server to provide a web-based interface for managing containerized services, with persistent storage and automatic restart enabled.

---

### Portainer Container Management
![Portainer Container Dashboard](screenshots/portainer-dashboard-containers.png)

Portainer dashboard showing the running Docker environment, allowing centralized visibility and management of containers, images, volumes, and networks.
