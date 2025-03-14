NGINX
=====

An Ansible role to install the [NGINX](https://www.nginx.com/) web server.

Requirements
------------

- Supported version of Ansible: 2.12 and higher. Systems with Python versions below than 3.7 are not compatible with ansible-core 2.17 (see [ansible/ansible#83357](https://github.com/ansible/ansible/issues/83357#issuecomment-2150254754)).
- Supported platforms:
  - Amazon Linux
    - 2 (only `mainline` release channel)
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

All variables that can be overridden are stored in the [defaults/main.yml](https://github.com/antmelekhin/ansible-role-nginx/blob/main/defaults/main.yml) file.
Please refer to the [meta/argument_specs.yml](https://github.com/antmelekhin/ansible-role-nginx/blob/main/meta/argument_specs.yml) file for a description of the available variables.
Similarly, descriptions and defaults for preset variables can be found in the [vars/main.yml](https://github.com/antmelekhin/ansible-role-nginx/blob/main/vars/main.yml) file.

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
