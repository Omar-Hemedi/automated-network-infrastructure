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

```

## ⚙️ Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/yourusername/hybrid-lab-infra.git
cd hybrid-lab-infra

### 2. Provision Virtual Machines with Terraform

Navigate to the `terraform` directory and initialize Terraform:

```bash
cd terraform
terraform init
terraform apply

### 3. Configure Servers with Ansible

Once the virtual machines are provisioned, use Ansible to automate the configuration of both Linux and Windows servers.

#### 🧩 Steps

```bash
# 1. Navigate to the ansible directory
cd ../ansible

# 2. Verify the inventory file contains the correct IP addresses
# (Edit inventory/hosts or inventory.ini depending on your setup)

# 3. Run the main playbook
ansible-playbook -i inventory playbooks/setup.yml

### 4. Automate Network Device Configuration with Python

Use the provided Python scripts to automate configuration and management of Cisco network devices within your GNS3 simulation.

#### 🐍 Steps

```bash
# 1. Navigate to the python scripts directory
cd ../python

# 2. Run the network automation script
python3 network_automation.py

## 📈 Future Enhancements

- Integrate continuous deployment pipelines using GitHub Actions or Jenkins  
- Add monitoring stack with Prometheus and Grafana for server and network health visualization  
- Automate Windows Server management more extensively using Ansible via WinRM  
- Implement security monitoring with IDS/IPS tools like Snort or Suricata  
- Develop REST API endpoints to trigger automation workflows using Flask or FastAPI  
- Expand network simulation to include firewalls, VPNs, and DMZ zones for advanced lab scenarios  
- Containerize some services for microservices architecture experimentation  
- Include automated backup and disaster recovery scripts for critical infrastructure components

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

## 👤 Author

Omar Hemedi Jumaa
[LinkedIn](https://linkedin.com/in/omar-hemed)




