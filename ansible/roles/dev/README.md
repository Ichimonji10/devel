dev
===

This role installs the pulpcore component of Pulp 3. It also creates and
customizes `/etc/pulp/server.yaml`.

If the `pulp_install_strategy` is `development`, then debug mode is enabled in
`/etc/pulp/server.yaml`. Otherwise, debug mode is disabled.

NOTE: `SECRET_KEY` is updated even if a value is already present!

Example Usage
-------------

```yaml
- hosts: all
  roles:
    - dev
```

Variables
---------

This role depends on the variables exported by the `pulp-user` role.
