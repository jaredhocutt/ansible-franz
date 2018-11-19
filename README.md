# Franz

Installs Franz.

## Requirements

None

## Role Variables

| Variable        | Required | Default  | Description                                                                                                                                                                                                                                     |
| --------------- | -------- | -------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `franz_version` | :x:      | `latest` | Using `latest` will always download the latest version of Atom. You can select a specific version from [here](https://github.com/meetfranz/franz/releases). The value should match the tag (i.e. Franz 5.0.0-beta.18 would be `v5.0.0-beta.18`) |

## Dependencies

None

## Example Playbook

```yaml
- hosts: localhost
  vars:
    atom_version: v5.0.0-beta.18
  roles:
      - jaredhocutt.franz
```
