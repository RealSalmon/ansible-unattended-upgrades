[![Build Status](https://travis-ci.org/RealSalmon/ansible-unattended-upgrades.svg?branch=master)](https://travis-ci.org/RealSalmon/ansible-unattended-upgrades)

RealSalmon.unattended-upgrades
==============================
Configure unattended upgrades

Requirements
------------
- Ubuntu 14.04
- Ansible 1.9

Role Variables
--------------
- unattended_upgrades_origins: [security, updates]
- unattended_upgrades_blacklist: false
- unattended_upgrades_remove_unused: true
- unattended_upgrades_auto_reboot: false
- unattended_upgrades_reboot_time: "02:00"
- unattended_upgrades_update_package_lists: 1
- unattended_upgrades_download_packages: 1
- unattended_upgrades_autoclean_interval: 7

Dependencies
------------
None

Example Playbook
----------------
    ---
    - hosts: all
      roles:
        - RealSalmon.unattended-upgrades

License
-------
BSD

Author Information
------------------
Ben Jones <ben@fogbutter.com>
