# test-connection

## Description

This role tests the connection to the VM to ensure it's active and reachable before proceeding with other tasks.

## Tasks

- Uses Ansible's `ping` module to check connectivity.

## Usage

Include this role in your playbook to verify VM connectivity:

```yaml
- name: Test VM Connection
  hosts: all
  roles:
    - test-connection
