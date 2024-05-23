
### 4. `install-docker` Role

```markdown
# install-docker

## Description

This role installs Docker on the server, allowing you to manage and deploy containers.

## Tasks

- Uses Docker's official installation script to install Docker.

## Usage

Include this role in your playbook to install Docker:

```yaml
- name: Install Docker
  hosts: all
  roles:
    - install-docker
