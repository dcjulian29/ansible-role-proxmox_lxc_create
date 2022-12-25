# Ansible Role: proxmox_lxc_create

[![CI](https://github.com/dcjulian29/ansible-role-proxmox_lxc_create/actions/workflows/ci.yml/badge.svg)](https://github.com/dcjulian29/ansible-role-proxmox_lxc_create/actions/workflows/ci.yml) [![GitHub Issues](https://img.shields.io/github/issues-raw/dcjulian29/ansible-role-proxmox_lxc_create.svg)](https://github.com/dcjulian29/ansible-role-proxmox_lxc_create/issues)

This an Ansible role to create LCX containers in a Proxmox Virtual Environment (PVE) cluster or stand-alone host. It can use either vztmpl or iso templates. It has the ability to add custom template during the process of creation. This role is super-custom to my environment and makes that assumption during execution, YMMV.

## Requirements

- Proxmox 7.x installed and configured.
- For a cluster, it should be fully installed and configured.

## Installation

To use, use `requirements.yml` with the following git source:

```yaml
---
roles:
- name: dcjulian29.proxmox_lxc_create
  src: https://github.com/dcjulian29/ansible-role-proxmox_lxc_create.git
  version: main
  ```

Then download it with `ansible-galaxy`:

```shell
ansible-galaxy install -r requirements.yml
```

## Dependencies

If using a later version of Ansible, then the `community.general` collection should be already present in order to have the correct Proxmox modules. This has been tested on the current 6.x version of this collection.

Proxmox VE 7.x as a single-node or cluster environment.

## Role Variables

TODO

## Example Playbook

The examples directory include one or more example playbooks.
