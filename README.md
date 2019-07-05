# Franz

This role handles installing Franz from a release archive.

## Requirements

The hosts you are targeting should have the following packages:

- gtar

## Role Variables

| Variable          | Required | Default      | Description                                                                                                                                                                                                                       |
| ----------------- | -------- | ------------ | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| franz_version     | &#9989;  | `latest`     | Using `latest` will always download the latest version of Franz. You can select a specific version from the Franz [releases page](https://github.com/meetfranz/franz/releases) (i.e. Franz 5.0.0-beta.18 would be v5.0.0-beta.18) |
| franz_install_dir | &#9989;  | `/opt/franz` | The location to unpack the Franz release archive and install Franz                                                                                                                                                                |

## Dependencies

None

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: jaredhocutt.franz
      vars:
         franz_version: v5.0.1
```

## License

MIT

## Author Information

Jared Hocutt (@jaredhocutt)
