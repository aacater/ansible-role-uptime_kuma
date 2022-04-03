# Ansible Role: Uptime Kuma

[![CI](https://github.com/aacater/ansible-role-uptime_kuma/workflows/CI/badge.svg?event=push)](https://github.com/aacater/ansible-role-uptime_kuma/actions?query=workflow%3ACI)
[![LICENSE](https://img.shields.io/badge/license-MIT-brightgreen.svg)](LICENSE)

Installs [Uptime Kuma](https://github.com/louislam/uptime-kuma).

## Requirements

NodeJS >= 14

## Role Variables

None.

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
