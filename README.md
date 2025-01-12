# Ansible Project for AppDynamics Installation and User Management

This project is designed to automate the installation of AppDynamics and the creation of user accounts with admin access using Ansible.

## Project Structure

- **ansible.cfg**: Configuration settings for Ansible.
- **inventory/hosts**: Defines the target hosts for the playbooks.
- **playbooks/appd_install.yml**: Playbook for installing AppDynamics.
- **roles/appd**: Role for managing AppDynamics installation.
  - **tasks/main.yml**: Tasks for downloading and installing AppDynamics.
  - **vars/main.yml**: Variables for the AppDynamics role.

## Requirements

- Ansible installed on your control machine.
- Access to the target hosts defined in the inventory file.
- Necessary permissions to install software and create users on the target hosts.
- Environment variables `APPD_USERNAME` and `APPD_LICENSE_KEY` set for AppDynamics installation.

## Setup Instructions

1. Clone the repository:
   ```sh
   git clone <repository-url>
   cd ansible-project