NGINX
=====

An Ansible role to install NGINX web server.

Requirements
------------

- Supported version of Ansible: 2.12 and highter.
- Supported platforms:
  - Debian
    - 10
    - 11
    - 12
  - RHEL
    - 7
    - 8
    - 9
  - Ubuntu
    - 18.04
    - 20.04
    - 22.04

Role Variables
--------------

- `nginx_version` The specific version of `NGINX` to install (default: `''`).
- `nginx_repository_mirror_url` Mirror of `NGINX` repository (default: `https://nginx.org/packages`).
- `nginx_repository_gpgkey_url` URL to `NGINX` GPG public key file (default: `https://nginx.org/keys/nginx_signing.key`).
- `nginx_repository_branch` `NGINX` release branch.

  Available values:
  - `stable` (default)
  - `mainline`

Dependencies
------------

None.

Example Playbook
----------------

- Install `NGINX`:

  ```yaml
  ---
  - name: 'Install NGINX'
    hosts: all

    roles:
      - role: antmelekhin.nginx
  ```

- Install a specific version of `NGINX`:

  ```yaml
    ---
  - name: 'Install NGINX v1.22.1'
    hosts: all

    roles:
      - role: antmelekhin.nginx
        nginx_version: '1.22.1-1~jammy'
        when: ansible_distribution == 'Ubuntu' and ansible_distribution_version is version('22.04', '=')

      - role: antmelekhin.nginx
        nginx_version: '1.22.1'
        when: ansible_os_family == 'RedHat'
  ```

License
-------

MIT

Author Information
------------------

Melekhin Anton.
