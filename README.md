# Hadoop Preparations

This is an Ansible Playbook with a few roles that is supposed to prepare servers for a Hadoop installation.

Currently it supports:

* CentOS (tested against 6.5 only)

## Running it

To run it against a local Vagrant machine (with SSH on port 2222) use the following command:

    ansible-playbook -i vagrant site.yml

## Roles

### Common

### Fetch Info

This role fetches relevant system files from all hosts. These are things like `/etc/hosts` and `/etc/resolv.conf`. That makes debugging problems easier.
