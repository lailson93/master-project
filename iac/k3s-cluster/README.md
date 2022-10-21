iac
===

K3S Ansible playbook based on https://github.com/k3s-io/k3s-ansible

### Introduction

This playbook creates a cluster `k3s` using `ansible` as a manager of tasks in vms.

### Project struture

```
+-- group_vars/            # Config envs
+-- roles/                 # Ansible roles
+-- site.yml               # Playbook
```

### Requirements

- [Ansible 2.4.0+](https://docs.ansible.com/ansible/2.4/intro_installation.html#latest-releases-via-pip) 
- Master and Nodes VMs must have SSH passwordless and a hostname settled.

### Start Playbook

```
ansible-playbook -i overlays/lab site.yml
```