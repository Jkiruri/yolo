
### 7. `deploy-containers` Role

```markdown
# deploy-containers

## Description

This role deploys Docker containers using a `docker-compose.yml` file.

## Tasks

- Copies the `docker-compose.yml` file to the server.
- Runs `docker-compose up` to start the containers.

## Variables

- `compose_file_src`: The local path to the `docker-compose.yml` file.
- `compose_file_dest`: The destination path on the server for the `docker-compose.yml` file.

## Usage

Include this role in your playbook to deploy Docker containers:

```yaml
- name: Deploy Docker Containers
  hosts: all
  vars:
    compose_file_src: "./docker-compose.yml"
    compose_file_dest: "/path/on/server/docker-compose.yml"
  roles:
    - deploy-containers
