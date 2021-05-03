# Backup Cisco Switches with Ansible

- Basic script to backup Cisco Switch Config Files. This script execute two tasks (create folder and backup a config .cfg file) in one yaml playbook file.

## Execution Requirements

- Tested with Ubuntu 18 terminal in a Windows 10 PC (works fine in linux enviroment).
- Tested with Ansible version 2.9
- Tested with Python version 2.7

## Target Requirements

- Cisco switches model 2960
- SSH version 2.0 or higher configured.

## Variables

- ./ansible.cfg -> Edit your host path if you want
- ./hosts -> Edit your ansible hosts/switches
- /group_vars/all.yml -> Edit your user and pass to access the targets via ssh. (Recommended for enviroment with TACACS+ or RADIUS servers)

## How to use

`ansible-playbook backup-cisco-switch.yml`

## What does this script do?

- Create a directory in the path C:/bkp_year-month-day/Switches/
- Backup all cisco switches config files of your enviroment
- Save each config file in the Switches folder

## Author Information

This role was created by [João Vitor Costa Medeiros](https://www.linkedin.com/in/joaovitorcm/)
