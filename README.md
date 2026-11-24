# Ansible Linux Server Automation

![Ansible](https://img.shields.io/badge/Ansible-Automation-EE0000?logo=ansible&logoColor=white)
![Linux](https://img.shields.io/badge/OS-Linux-FCC624?logo=linux&logoColor=black)
![Ubuntu](https://img.shields.io/badge/Control_Node-Ubuntu-E95420?logo=ubuntu&logoColor=white)
![Debian](https://img.shields.io/badge/Managed_Node-Debian-A81D33?logo=debian&logoColor=white)
![Status](https://img.shields.io/badge/Project-In_Progress-yellow)

## 📌 Project Overview

This project demonstrates Linux server automation and configuration management using **Ansible**.

The objective is to automate common Linux system administration tasks, manage remote servers, and simplify infrastructure operations using Ansible Playbooks.

The project is implemented in a virtualized laboratory environment using Oracle VirtualBox.

## 🏗️ Infrastructure Architecture

| Component | Configuration |
|---|---|
| Control Node | Ubuntu Linux |
| Managed Node | Debian 13 |
| Virtualization | Oracle VirtualBox |
| Automation Tool | Ansible |
| Communication | SSH |
| Configuration Language | YAML |

### Architecture Diagram

```text
          ADMINISTRATOR
                |
                |
         UBUNTU CONTROL NODE
             voldemort
                |
                |
             ANSIBLE
                |
                |
          SSH CONNECTION
                |
                |
          DEBIAN 13 SERVER
           MANAGED NODE
                |
                |
       AUTOMATED ADMINISTRATION
```

## 🛠️ Technologies Used

- Ansible
- Ubuntu Linux
- Debian Linux
- SSH
- YAML
- Oracle VirtualBox
- Linux Command Line

## 🚀 Implementations

### 1. Ansible Installation and Configuration

Installed Ansible on the Ubuntu control node and prepared the environment for remote Linux server management.

### 2. SSH Connectivity

Configured SSH communication between the Ubuntu control node and Debian managed node.

### 3. Inventory Management

Created an Ansible inventory file to define and organize managed Linux hosts.

### 4. Ansible Ad-hoc Commands

Practiced executing remote administrative commands using Ansible.

Examples include:

- Package installation
- Remote command execution
- System administration tasks

### 5. Ansible Playbooks

Developed YAML-based playbooks to automate Linux administration tasks.

## 📂 Repository Structure

```text
ansible-linux-automation/
│
├── README.md
│
├── inventory/
│   └── inventory.ini
│
├── playbooks/
│   ├── install_packages.yml
│   ├── update_system.yml
│   ├── create_users.yml
│   └── install_node_exporter.yml
│
├── screenshots/
│
└── documentation/
    ├── architecture.md
    └── troubleshooting.md
```

*Additional directories and playbooks will be added as the project progresses.*

## 🎯 Project Objectives

- Automate Linux server administration.
- Manage multiple Linux servers using Ansible.
- Implement configuration management.
- Automate package installations and system updates.
- Deploy monitoring agents using Ansible.
- Integrate infrastructure automation with Prometheus and Grafana.

## 📈 Future Enhancements

- Automated Linux package management.
- Automated user and group management.
- Automated Node Exporter installation.
- Multi-server configuration management.
- Prometheus monitoring integration.
- Grafana infrastructure monitoring integration.
- GitHub Actions for Ansible playbook validation.

## 👨‍💻 Author

**John Paul Javier**

IT Infrastructure Engineer | Linux | Ansible | Grafana | Prometheus | Splunk | AWS

GitHub: https://github.com/johnpauljavier

---

⭐ This project is part of my continuous learning journey in Linux Administration, Infrastructure Automation, and DevOps.
