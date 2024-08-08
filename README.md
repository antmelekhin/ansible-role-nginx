NGINX
=====

An Ansible role to install the [NGINX](https://www.nginx.com/) web server.

Requirements
------------

- Supported version of Ansible: 2.12 and highter.
- Supported platforms:
  - Amazon Linux
    - 2
    - 2023
  - Debian
    - 10
    - 11
    - 12
  - Fedora
    - 39
    - 40
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

- `nginx_version` The version of the NGINX package. By default, NGINX is installed with the latest available version.
- `nginx_repository_mirror_url` The NGINX repository mirror (default: `https://nginx.org/packages`).
- `nginx_repository_gpgkey_url`URL to NGINX repository GPG key file (default: `https://nginx.org/keys/nginx_signing.key`).
- `nginx_repository_branch` NGINX repository release channel. Available values are: `stable` (default), `mainline`.

Dependencies
------------

None.

Example Playbook
----------------

Install NGINX:

```yaml
---
- name: 'Install NGINX'
  hosts: all

  roles:
    - role: antmelekhin.nginx
```

Install NGINX v1.22.1:

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
