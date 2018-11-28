# Changes and migration requirements

## Version 0.0.4

*Note: When upgrading from 0.0.2 or earlier to 0.0.4, test startup after reboot
and deploying with/without uWSGI running at the time.  The init script changes
might be ineffective for intervals due to caching by systemd.  Running
`sudo systemctl daemon-reload` might help, but rebooting may be necessary.*

* Simplify enabling/starting uWSGI.  (Switch a command-line invocation to the
  appropriate Ansible module(.

## Version 0.0.3

* Fix a problem with the init script which prevented uWSGI from starting at
  system boot on Ubuntu 18.04.

## Version 0.0.2

* Remove stray text in LICENSE
