# ansible-pgsql-demo

An Ansible playbook to deploy postgresql in a master - slave replication configuration.

The goal of this playbook is to demonstrate how fast & easy it can be to deploy applications with high availability into the cloud using Ansible.

## Setup

### Prerequisites

```
make
```


### SSH key setup

Your SSH RSA public key must be present at the following location: '~/.ssh/id_rsa.pub'

### Variable setup

A few variables must be setup prior executing this playbook. These variables are located in the following file:

```
default/main.yml
```


## Running the playbook 

To run the playbook:

```
ansible-playbook -v role.yml 
```

## Notice

This playbook has been tested only on Ubuntu 14.04.

It is inspired from [this] (https://github.com/lesovsky/ansible-postgresql-on-el6) playbook.
