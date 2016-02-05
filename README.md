# Ansible role for Rabbitmq

Playbook to install and configure rabbitmq. Will come with various configuration tweaking later on.

If you wish to discuss modifications, or help to support more platforms, open an issue.

## Tested On

  * Ubuntu 14.04

## Defaults

The `defaults/main.yml` should be pretty clear on the usage and values. The 
version used by defaults are:

  * `rabbitmq_config_dir`: /etc/rabbitmq
  * `rabbitmq_port`: 5672
  * `rabbitmq_ip`: 127.0.0.1

## Usage

The tests in the respository should be pretty straight forward, but here are
some examples:

### Rabbitmq

playbook.yml:

```
- name: Install and run rabbitmq
  hosts: all
  sudo: True

  roles:
    - { role: ansible-rabbitmq }

```

## TODO

  * Extract supervisor to it's own role
  * Extend to other distros

