# Ansible Role: Oracle Java [Ansible Playbook Role To Install Java]

Install Oracle Java 1.8, a distributed version control system, on any RHEL/CentOS Linux system.

## Requirements

None.

## Role Variables
None

## Dependencies

None.

## Usage and Example Playbook

Install from Ansible Galaxy

$ ansible-galaxy install avinash6784.oracle-java
Or download manually

$ git clone https://github.com/avinash6784/ansible-oracle-java.git 
The code should reside in the roles directory of ansible ( See ansible documentation for more information on roles ), in a folder oracle-java.

## Run the playbook

First create a playbook including the git role, naming it java.yml.
```yml
- name: Install Oracle Java
  hosts: java
  become: true
  roles:
    - oracle-java
    
$ ansible-playbook -i hosts java.yml
```

## Author Informations

This role was created by [Avinash Pawar](https://github.com/avinash6784/ansible-oracle-java).
