# Ansible Role: Oracle Java [Ansible Playbook Role To Install Java]

Install Oracle Java 1.8, a distributed version control system, on any RHEL/CentOS Linux system.

## Requirements

None.

## Role Variables
```yml

#Role Java vars
download_url: http://download.oracle.com/otn-pub/java/jdk/8u151-b12/e758a0de34e24606bca991d704f6dcbf/jdk-8u151-linux-x64.tar.gz
download_folder: /opt
java_name: "{{download_folder}}/jdk1.8.0_151"
java_archive: "{{download_folder}}/jdk-8u151-linux-x64.tar.gz"
java_env_file: "/etc/profile.d/java.sh"
java_home: /opt/jdk1.8.0_151

```

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

This role was created by [Avinash Pawar](http://devopstechie.com).
