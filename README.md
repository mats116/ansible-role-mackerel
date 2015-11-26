# README.md
# Ansible Role: mats116.mackerel-agent

An Ansible role that installs mackrel-agent on **Ubuntu 14.04 LTS**

## Requirements

none

## Role Variables

Available variables are listed below, along with default values:

```yaml
mackerel_service: default
mackerel_role: default

mackerel_auto_retirement: 0

mackerel_plugin_conf: []
```

## Dependencies

none

## Example Playbook

```yaml
- hosts: web-server
  roles:
    - role: mats116.mackerel-agent
      mackerel_auto_retirement: 1
      mackerel_plugin_conf:
        - nginx.conf
```

## License

MIT
