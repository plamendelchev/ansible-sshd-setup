# sshd Setup

Ansible Role for Setting Up sshd on EL-based Linux distributions. The role has not been tested on non EL-based distributions. 

## Role Variables

- sshd_config_client_alive_count `default: 3`
- sshd_config_client_alive_internal `default: 60`
- sshd_config_name `default: 00_custom.conf`
- sshd_config_port `default: 22`

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: ansible-sshd-setup
      vars:
        sshd_config_port: 9786
```

## License

GPL-3.0
