
### 5. `install-git` Role

```markdown
# install-git

## Description

This role installs Git on the server, enabling the cloning of repositories.

## Tasks

- Uses `apt-get install git` to install Git.

## Usage

Include this role in your playbook to install Git:

```yaml
- name: Install Git
  hosts: all
  roles:
    - install-git
