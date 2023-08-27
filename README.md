NGINX
=====

An Ansible role that installs NGINX web server.

Requirements
------------

- Supported version of Ansible: 2.9 and highter.
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

- `nginx_package_version` The specific version of `NGINX` to install (default: `''`).
- `nginx_repository_mirror` Mirror of `NGINX` repository (default: `https://nginx.org/packages`).
- `nginx_repository_key_url` URL to `NGINX` GPG public key file (default: `https://nginx.org/keys/nginx_signing.key`).
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

License
-------

MIT

Author Information
------------------

Melekhin Anton.
