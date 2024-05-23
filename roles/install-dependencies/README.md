# install-dependencies

## Description

This role installs all the necessary dependencies required for the application to run. These dependencies may include various tools and libraries needed for both the backend and frontend components.

## Tasks

- Updates the package list to ensure the latest versions of packages are available.
- Installs common build tools and libraries.
- Installs other required dependencies specific to the application.

## Variables

You can define specific dependencies to be installed by this role by setting the `dependencies` variable in your playbook. For example:

```yaml
dependencies:
  - build-essential
  - curl
  - git
  - libssl-dev
  - python3
  - python3-pip
