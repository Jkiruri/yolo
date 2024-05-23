
### 2. `update-server` Role

```markdown
# update-server

## Description

This role updates the server's package index and upgrades all installed packages to their latest versions.

## Tasks

- Runs `apt-get update` to update the package index.
- Runs `apt-get upgrade` to upgrade installed packages.

## Usage

Include this role in your playbook to update and upgrade the server:

```yaml
- name: Update and Upgrade Server
  hosts: all
  roles:
    - update-server
