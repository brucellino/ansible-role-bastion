# Ansible Role Bastion

This role creates a [Bastion host](https://en.wikipedia.org/wiki/Bastion_host), typically for use in a cloud environment.
This is essentially a secure SSH server, configured to protect a subnet behind it.
This role builds [OpenSSH from scratch](https://ftp.openbsd.org/pub/OpenBSD/OpenSSH/portable/INSTALL) so that you have full control over it.

## Requirements

The role is tested on AWS EC2, so you will need `boto`.

## Role Variables

Role variables are kept in [`defaults/main.yml`](defaults/main.yml) unless overwritten by site, group, or other vars.

Important variables are:

- `prerequisites` - OS-specific packages which are needed in order to install OpenSSH.
- `ssh` - variables to configure OpenSSH itself.

## Dependencies

## Example Playbook

    - hosts: servers
      roles:
         - { role: brucellino.bastion }

## License

MIT

## Author Information

Bruce Becker | bruce.becker@aptus.eu
