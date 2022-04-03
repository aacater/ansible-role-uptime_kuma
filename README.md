# Ansible Role: Uptime Kuma

[![CI](https://github.com/aacater/ansible-role-uptime_kuma/workflows/CI/badge.svg?event=push)](https://github.com/aacater/ansible-role-uptime_kuma/actions?query=workflow%3ACI)
[![LICENSE](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE)

Installs [Uptime Kuma](https://github.com/louislam/uptime-kuma).

## Requirements

- NodeJS >= 14

## Role Variables

Available variables are listed below, along with default values (see [defaults/main.yml](defaults/main.yml)):

    uptime_kuma_version: 1.13.1

The version of uptime kuma to install.

    install_git: true

This role uses the [package module](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/package_module.html) to install git. Set `install_git` to false if you want to skip this and install git manually.

    uptime_kuma_git: https://github.com/louislam/uptime-kuma

Url of git repository that will be cloned.

    uptime_kuma_user: kuma
    uptime_kuma_group: kuma

User and group names to install uptime kuma as.

    uptime_kuma_app: /opt/uptime-kuma/app

The location to install uptime kuma.

    uptime_kuma_data: /opt/uptime-kuma/data

The location to store data for uptime kuma.

## Dependencies

None.

## Example Playbook

    - hosts: servers
      roles:
        - geerlingguy.nodejs
        - aacater.uptime_kuma

## License

MIT

## Author Information

This role was created in 2022 by [Alex Cater](https://www.aacater.net/).
