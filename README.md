# Ansible Install Docker CE Role

An Ansible role to install Docker CE on Ubuntu.

## Rationale for this role

For some reason, all docker-related roles that I could find in Ansible Galaxy install the `docker-engine` package, which is an outdated package. The latest Docker docs refer to the `docker-ce` package.

## Requirements

This role requires Ansible 1.2 or higher.

It only applies to Ubuntu Trusty, Xenial or Yakketty.

## Role variables

* `docker_key_server`: the url of the Docker GPG key

## Installation

```
ansible-galaxy install opichon.install-docker-ce
```

## Usage

Add the role to your playbook.

```
---
- name: Install Docker CE
  role: opichon.install-docker-ce
```
