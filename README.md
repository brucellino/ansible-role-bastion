# Ansible Role Bastion

This role creates a [Bastion host](https://en.wikipedia.org/wiki/Bastion_host), typically for use in a cloud environment

## Requirements

The role is tested on AWS EC2, so you will need `boto`.

## Role Variables


## Dependencies


## Example Playbook


    - hosts: servers
      roles:
         - { role: brucellino.bastion }

## License

MIT

## Author Information

Bruce Becker | bruce.becker@aptus.eu