# Ansible Role: timezone

An Ansible Role to update the timezone.

[![Actions Status](https://github.com/tristan-weil/ansible-role-timezone/workflows/molecule/badge.svg?branch=master)](https://github.com/tristan-weil/ansible-role-timezone/actions)

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

Mandatory variables:

| Variable      | Description |
| :------------ | :---------- |

Optional variables:

| Variable      | Default | Description |
| :------------ | :------ | :---------- |
| timezone_config | Etc/UTC | the timezone (must exist on the machine) |
| timezone_restat_cron | True | *True / False*: restart the cron service if the timezone is changed |

## Example Playbook

    - hosts: 'webservers'
      roles:
        - role: 'ansible-role-timezone'
          timezone_config: Etc/GMT-5

## Todo

None.

## Dependencies

None.

## Supported platforms

See [meta/main.yml](https://github.com/tristan-weil/ansible-role-timezone/blob/master/meta/main.yml)

## License

See [LICENSE.md](LICENSE.md)
