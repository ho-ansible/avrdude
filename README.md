# Ansible role: avrdude
Driver for AVR programmers for Arduino et al.
Permissions on the given USB devices will be assigned to the `plugdev` group.

## Requirements
Only tested on Debian stable, for now.

## Role Variables
+ `avrdude_usbids`: list of dicts: 
  + `name`: identifying label for the AVR programmer
  + `vendor`: USB vendor ID (4 hex digits)
  + `product`: USB product ID (4 hex digits)

## Playbooks
+ `main.yml`: apply role
+ `uninstall.yml`: remove. Run prior to removing host from inventory group.

## Dependencies
None.

## License
+ Ansible role licensed [MIT](LICENSE)

## Author Information
+ Ansible role by [Sean Ho](https://github.com/ho-ansible/)
+ [AVRDUDE](https://github.com/avrdudes/avrdude) is by Brian S. Dean, Jörg Wunsch, and other contributors
