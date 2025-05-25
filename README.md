# automated-network-infrastructure
Automated hybrid lab environment combining Cisco networking, Windows and Linux server administration, and infrastructure automation with Terraform, Ansible, and Python. Demonstrates real-world skills in network engineering, system administration, and DevOps automation.

# Hybrid Lab Infrastructure Automation

## 🚀 Project Overview

This project simulates a **hybrid enterprise IT environment** combining Cisco networking with automated provisioning and configuration of Windows and Linux servers. It showcases expertise in **network engineering**, **system administration**, and **infrastructure automation** using industry-standard tools like **Terraform**, **Ansible**, and **Python**.

The goal is to build a scalable, secure lab environment with real-world components and automation that can be easily deployed and managed.

---

## 🔧 Skills Demonstrated

- **Network Engineering (Cisco)**
  - VLANs, Inter-VLAN routing, OSPF, ACLs
  - Site-to-site VPN setup using Cisco routers (GNS3)
  - Network segmentation and security best practices

- **System Administration**
  - Windows Server: Active Directory, DHCP, DNS, Group Policy Objects (GPO)
  - Ubuntu Server: LAMP stack, SSH hardening, user management

- **Infrastructure Automation
  - Infrastructure provisioning with **Terraform** (VMware/virtual environment)
  - Configuration management with **Ansible** (Linux & Windows)
  - Network automation using **Python** (Netmiko/NAPALM)
  - Scripted deployment and monitoring tools

---

## 🏗️ Infrastructure Architecture

                  [Cisco GNS3 Network Simulation]
                             │
           ┌─────────────────┴─────────────────┐
           │                                   │
   [Ubuntu Server VM]                   [Windows Server VM]
           │                                   │
 Configured & Managed via               Joined to Active Directory
      Ansible Playbooks

  
---

## 📂 Repository Structure

```plaintext
├── ansible/               # Ansible playbooks and inventory files
│   ├── playbooks/
│   └── inventory/
├── terraform/             # Terraform configuration files
│   ├── main.tf
│   └── variables.tf
├── python/                # Python scripts for network automation
│   └── network_automation.py
├── diagrams/              # Network topology and architecture diagrams
│   └── lab_topology.png
├── scripts/               # Helper scripts (e.g., setup scripts)
│   └── setup.sh
├── README.md              # Project documentation
└── LICENSE                # License file (MIT)


