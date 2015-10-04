Role Name
=========

`bosh-init` is a tool used to create and update the Director (its VM and persistent disk) in a BOSH environment.

Read details:

* [bosh-init project page](https://github.com/cloudfoundry/bosh-init)
* [install bosh-init](https://bosh.io/docs/install-bosh-init.html)

Requirements
------------

This Role is tested with Ansible 1.9.

Role Variables
--------------

`bosh_init_version` - version of bosh-init to install.
`bosh_init_url` - URL to fetch bosh-init binary.
See `defaults/main.yml` for defaults.

Example Playbook
----------------

```yaml
- hosts: jumpbox
  roles:
     - { role: allomov.bosh-init, bosh_init_version: 0.0.74 }
```

Author Information
------------------

Alexander Lomov - lomov.as@gmail.com
