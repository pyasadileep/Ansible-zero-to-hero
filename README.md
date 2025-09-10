# Ansible Playbooks Portfolio

This repository contains Ansible playbooks demonstrating my proficiency from beginner to advanced levels. The playbooks are organized as:

- **basics/**: Simple tasks like package installation and user creation.
- **intermediate/**: More complex automation, using templates, variables, and multi-task playbooks.
- **advanced/**: Advanced orchestration including Docker deployment and cloud provisioning.
- **roles/**: Modular Ansible roles following best practices.

## Usage

## 1. Clone the repository:
```bash
git clone https://github.com/<username>/ansible-playbooks-portfolio.git
cd ansible-playbooks-portfolio


## Run a playbook:

ansible-playbook -i inventory.ini basics/install_apache.yml


Customize inventory and variables as needed.


---

## **2. Inventory File: `inventory.ini`**

```ini
[webservers]
192.168.1.10

[app_servers]
192.168.1.20

Replace IPs with your test VMs or cloud instances.
[database]
192.168.1.30
