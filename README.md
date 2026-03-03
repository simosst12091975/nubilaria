1. Project Title & Description
# Project Nubilaria Automation
This repository contains Ansible Playbooks for automating the deployment and configuration of the Nubilaria environment. It is designed to be executed via Semaphore UI. 
2. Getting Started
Prerequisites
Ansible: v2.10+
Semaphore UI: Access to a running instance.
Target Systems: SSH access to hosts defined in the Inventory. 
Repository Structure
playbooks/: Core automation files.
roles/: Reusable Ansible Roles.
inventory/: Host definitions (if using file-based inventory).
requirements.yml: External dependencies for ansible-galaxy. 
3. Semaphore UI Configuration
To run this project, configure the following in your Semaphore Project:
Key Store: Add an SSH key (for server access) and a "Login with Password" key (for GitHub PAT).
Inventory: Point to inventory/hosts.ini or use a "Static" inventory in the UI.
Environment: Add necessary extra-vars (e.g., app_version).
4. Available Playbooks
site.yml: Main deployment playbook.
db_setup.yml: Configures the database cluster.
web_deploy.yml: Updates frontend application code.
5. Contribution & Support
Fork the repository.
Create a feature branch (git checkout -b feature/awesome-fix).
Commit your changes and open a Pull Request. 
Author: [Stefano Mosso/Team]
License: MIT
