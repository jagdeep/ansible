# Ansible for Workstation Setup on Fedora 32

## Install Ansible
```
sudo yum install ansible
```

## Install Ansible Community Collection

The collection is a part of the Ansible package and includes many modules and plugins supported by Ansible community which are not part of more specialized community collections.

```
ansible-galaxy collection install community.general
```
