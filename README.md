# Ansible Role: NGINX

[![role: ubzyhd.nginx](https://img.shields.io/ansible/role/42671?color=blueviolet&logo=ansible&style=flat-square)](https://galaxy.ansible.com/ubzyhd/nginx)

![Description from Ansible](https://img.shields.io/badge/dynamic/json?label=Description&style=flat-square&query=description&url=https%3A%2F%2Fgalaxy.ansible.com%2Fapi%2Fv1%2Fcontent%2F42671%2F)

[![GitHub release](https://img.shields.io/github/release/ubzyhd/ansible-role-nginx)](https://GitHub.com/ubzyhd/ansible-role-nginx/releases/) [![GitHub tag](https://img.shields.io/github/tag/ubzyhd/ansible-role-nginx)](https://GitHub.com/ubzyhd/ansible-role-nginx/tags/)

[![HitCount](http://hits.dwyl.io/ubzyhd/ansible-role-nginx.svg)](http://hits.dwyl.io/ubzyhd/ansible-role-nginx)
## Contents

- [Ansible Role: NGINX](#ansible-role-nginx)
  - [Contents](#contents)
  - [Role Info & Build Status](#role-info--build-status)
  - [Supported OS's](#supported-oss)
  - [Role Variables](#role-variables)
  - [Example Playbook](#example-playbook)
  - [License](#license)
  - [Author Information](#author-information)
  - [Credits](#credits)

## Role Info & Build Status

|Branch             | Master | Development |
|-------------------|:--------:|:--------------:|
| Build Status:      | [![travis-ci build status](https://img.shields.io/travis/UbzyHD/ansible-role-nginx/master?label=build&logo=travis-ci&style=flat-square)](https://travis-ci.org/UbzyHD/ansible-role-nginx)       |              |
| Ansible Version: | [![https://galaxy.ansible.com/ubzyhd/nginx](https://img.shields.io/badge/dynamic/json?color=red&style=flat-square&label=Minimum%20Ansible%20Version%3A&query=min_ansible_version&url=https%3A%2F%2Fgalaxy.ansible.com%2Fapi%2Fv1%2Fcontent%2F42671%2F)](https://galaxy.ansible.com/ubzyhd.nginx)       |              |
| Statistics:  | [![https://galaxy.ansible.com/ubzyhd/nginx](https://img.shields.io/ansible/role/d/42671?color=blue&logo=ansible&style=flat-square)](https://galaxy.ansible.com/ubzyhd.nginx)<br>[![https://galaxy.ansible.com/ubzyhd/nginx](https://img.shields.io/badge/dynamic/json?color=blue&logo=ansible&style=flat-square&label=Quality%20Score:&query=quality_score&url=https%3A%2F%2Fgalaxy.ansible.com%2Fapi%2Fv1%2Fcontent%2F42671%2F)](https://galaxy.ansible.com/ubzyhd.nginx)<br>[![https://galaxy.ansible.com/ubzyhd/nginx](https://img.shields.io/badge/dynamic/json?color=blue&logo=ansible&style=flat-square&label=Content%20Score%3A&query=content_score&url=https%3A%2F%2Fgalaxy.ansible.com%2Fapi%2Fv1%2Fcontent%2F42671%2F)](https://galaxy.ansible.com/ubzyhd.nginx)<br>[![https://galaxy.ansible.com/ubzyhd/nginx](https://img.shields.io/badge/dynamic/json?color=blue&logo=ansible&style=flat-square&label=Metadata%20Score%3A&query=metadata_score&url=https%3A%2F%2Fgalaxy.ansible.com%2Fapi%2Fv1%2Fcontent%2F42671%2F)](https://galaxy.ansible.com/ubzyhd.nginx)       |              |

## Supported OS's

Debian:

- 10 - Buster
- 9 - Jessie

## Role Variables

This role has no variables.

## Example Playbook

An example playbook with all the variables can be found called ```example-playbook-nginx.yml```

or here:

```yaml
---
- name: UbzyHD.NGINX Example Playbook
  hosts: all
  order: sorted

  gather_facts: true
  any_errors_fatal: true

  pre_tasks:

    - name: UbzyHD.NGINX Example Playbook | Pinging hosts.
      action: ping

    - name: UbzyHD.NGINX Example Playbook | Install Python if not already present.
      raw: test -e /usr/bin/python || (apt -y update && apt install -y python-minimal)
      changed_when: false

    - name: UbzyHD.NGINX Example Playbook | Gather facts after Python is definitely present.
      setup:

  roles:
    - ubzyhd.nginx
```

## License

MIT

## Author Information

This role was creating by Ubzy in 2019

## Credits

Jeff Geerling:

- [GitHub - geerlingguy](https://github.com/geerlingguy)
- [Website - jeffgeerling.com](https://www.jeffgeerling.com/)

>Without using his roles as the basis for mine, it wouldn't have been possible for me to create them.
