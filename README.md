# Ansible for Fedora 35
Ansible for a Fedora 35 workstation Setup using ansible-pull

## Install Ansible

Ansible is an IT automation tool. It can configure systems, deploy software, and orchestrate more advanced IT tasks such as continuous deployments or zero downtime rolling updates.

```
sudo yum install ansible
```

## Install Ansible Community Collection

The collection is a part of the Ansible package and includes many modules and plugins supported by Ansible community which are not part of more specialized community collections.

```
ansible-galaxy collection install community.general
```

## Execute Ansible Playbook

This pulls playbooks from a VCS repo and executes them for the local host

```
sudo ansible-pull -U https://github.com/jagdeep/ansible-fedora-35.git
```

# Extras

## Install Oracle Instant Cleint with sqlplus
```
sudo ansible-playbook oracle.yml
```

## Install docker and docker compose
```
sudo ansible-playbook docker.yml
```

## Install Ansible role for rvm
It is an Ansible role to install and manage ruby versions using rvm.
```
ansible-galaxy install rvm.ruby
```

## Fish themes
https://github.com/oh-my-fish/oh-my-fish
```
curl https://raw.githubusercontent.com/oh-my-fish/oh-my-fish/master/bin/install | fish
```
