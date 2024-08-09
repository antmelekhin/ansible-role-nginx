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

All variables that can be overridden are stored in the [defaults/main.yml](defaults/main.yml) file.
Please refer to the [meta/argument_specs.yml](meta/argument_specs.yml) file for a description of the available variables.
Similarly, descriptions and defaults for preset variables can be found in the [vars/main.yml](vars/main.yml) file.

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
