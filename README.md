### Ansible Database ware

Ansible roles for installing and setting up different web ware
on Debian/Ubuntu and Archlinux.

### Install
Add this repo as a submodule in your `roles/` folder and include it in
a playbook of yours.

### Config example
```yaml
---
webserver: apache

work_dir: /srv/http/www

apache:
  version: 2.4
  port: 80
  modules:
    - rewrite
    - expires
  group_users:
    - git
    - rafi
    - adam
    - ronen
    - yakir
    - yaniv
```

### License
MIT
