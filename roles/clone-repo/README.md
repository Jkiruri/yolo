
### 6. `clone-repo` Role

```markdown
# clone-repo

## Description

This role clones the project repository into the server, preparing it for deployment.

## Tasks

- Uses Ansible's `git` module to clone the repository.

## Variables

- `repo_url`: The URL of the repository to clone.
- `dest_dir`: The destination directory on the server where the repository should be cloned.

## Usage

Include this role in your playbook to clone a repository:

```yaml
- name: Clone Project Repository
  hosts: all
  vars:
    repo_url: "https://github.com/Jkiruri/yolo.git"
    dest_dir: "/path/to/clone"
  roles:
    - clone-repo
