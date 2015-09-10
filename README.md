Synergy
=========

Install synergy from a package t role. The package is copied to `/opt/` on target host. It creates a synergy user group

Requirements
------------

Place your synergy package inside the `file` directory. this role might not be the latest. Fork it 'n update if needed.

Role Variables
--------------

The paths where binaries and log files are. This is to change the group to synergy.

```yaml
synergy_binary_paths:
  - /usr/bin/synergy
  - /usr/bin/synergyd
  - /usr/bin/synergyc
  - /usr/bin/synergys
  - /var/log/synergy.log
```

And the name of your package:

```yaml
synergy_package: synergy-v1.7.4-stable-c734bab-Linux-x86_64.rpm
```

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: archf.synergy }

If you want to add yor user to

License
-------

MIT

Author Information
------------------

Felix Archambault
