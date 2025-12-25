# Homelab Portfolio

This repository documents my personal homelab environment, built to simulate a real-world enterprise IT infrastructure using virtualization, Windows and Linux servers, centralized identity management, and containerized services.

---

## Lab Overview & Objectives

This homelab is designed to simulate a small-to-mid-sized enterprise IT environment, combining on-premises infrastructure, identity management, Linux services, and containerized workloads. The goal of the lab is to gain hands-on experience with real-world system administration tasks while following industry best practices for deployment, verification, and documentation.

Key objectives of this homelab include:
- Deploying and managing virtualized infrastructure using Proxmox VE
- Administering both Windows and Linux server operating systems
- Implementing centralized identity and access management with Active Directory
- Practicing role-based access control (RBAC) using users, groups, and OUs
- Deploying and validating containerized services using Docker
- Managing containers through Portainer for visibility and lifecycle control
- Verifying configurations using command-line tools and PowerShell
- Documenting workflows to mirror real-world operational practices

This lab emphasizes **installation, verification, and administration**, reflecting how systems are built, validated, and maintained in professional IT environments.

---

## Lab Implementation & Screenshots

### Proxmox Virtualization Host
![Proxmox Server](screenshots/proxmox-server.png)

Proxmox VE serves as the core virtualization platform for the homelab, providing centralized virtual machine management, snapshots, and resource allocation for all hosted systems.

---

### Windows Server Deployment
![Windows Server Installation](screenshots/windows-server-installation.png)

Microsoft Windows Server deployed as a virtual machine within the Proxmox environment. This system provides the foundation for enterprise identity services and Windows-based server administration.

---

## Active Directory Domain Services (AD DS)

### AD DS Installation
![Active Directory Installation](screenshots/active-directory-role-installation.png)

Active Directory Domain Services installed on Windows Server using PowerShell to enable centralized identity and access management.

---

### AD Service Verification
![Active Directory NTDS Service Running](screenshots/active-directory-ntds-service-running.png)

The NTDS service verified as running via PowerShell, confirming a successful AD DS installation.

---

### Domain Creation and Verification
![Active Directory Domain Details](screenshots/active-directory-domain-created.png)

Windows Server promoted to a domain controller, with the Active Directory domain created and validated using PowerShell.

---

### AD Object Management (Users, Groups, and OUs)
![Active Directory OUs](screenshots/active-directory-ou-structure.png)

Organizational Units created to logically separate domain controllers and user accounts in a scalable Active Directory structure.

![Active Directory Groups](screenshots/active-directory-group-membership.png)

Security groups created and managed using PowerShell, with users assigned to role-based groups to demonstrate RBAC and centralized permission management.

---

### Ubuntu Server Deployment
![Ubuntu Server Install](screenshots/Ubuntu%20Server%20Install.png)

Ubuntu Server LTS deployed as a virtual machine for Linux server administration, service hosting, and command-line management.

---

### Ubuntu Static IP Configuration
![Ubuntu Static IP](screenshots/Ubuntu%20Server%20-%20Static%20IP%20Creation.png)

A static IP configuration applied to ensure consistent network access, reflecting real-world server environments where predictable addressing is required.

---

## Docker & Container Management

### Docker Installation Verification
![Docker Hello World](screenshots/docker-hello-world-test.png)

Docker installation verified using the official `hello-world` container, confirming successful client–daemon communication, image retrieval, and container execution.

---

### Portainer Deployment via Docker
![Portainer Install](screenshots/portainer-install-docker.png)

Portainer CE deployed as a Docker container on Ubuntu Server to provide web-based container management with persistent storage and automatic restart configuration.

---

### Portainer Container Management
![Portainer Container Dashboard](screenshots/portainer-dashboard-containers.png)

Portainer dashboard displaying the Docker environment, enabling centralized monitoring and management of containers, images, volumes, and networks.
