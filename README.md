## Synopsis
This is an ansible role used to deploy and configure [shellinabox](https://github.com/shellinabox/shellinabox)

## Requirements

If using on a RedHat/CentOS-based host, make sure you've added the EPEL repository (it can easily be installed by including the `geerlingguy.repo-epel` role on Ansible Galaxy).  If wanting to use Apache for reverse proxy then this should also be installed prior to installation.

## Playbook example

This is used to deploy shellinabox to a jumphost server

```
---
- name: deploy and configure shellinabox
  hosts: ansible

  roles:

  - ansible-role-shellinabox
```
