unattended-upgrades
=========

_Installs unattended-upgrades._

Requirements
------------

Ansible 2.5 or above is highly recommended.

Role Variables
--------------

    unattended_upgrades_enabled: True
    unattended_upgrades_state: installed
    unattended_upgrades_unattended_upgrade: 1
    unattended_upgrades_autoclean_interval: 7
    unattended_upgrades_mailto: root
    unattended_upgrades_remove_old_kernels: true
    unattended_upgrades_remove_unused_dependencies: true
    unattended_upgrades_automatic_reboot: true
    unattended_upgrades_automatic_reboot_time: "02:00"

Dependencies
------------

    hyperized.package

Example Playbook
----------------

    - hosts: all
      become: yes
      roles:
        - role: hyperized.unattended-upgrades

License
-------

MIT

Author Information
------------------

Gerben Geijteman <gerben@hyperized.net>
