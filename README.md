Role Name
=========

Not complete role to create systemd timers

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      tasks:
        include_role:
          name: privx_de.systemd-timer
        vars:
          timer_name: backup-job
          timer_on_boot_sec: 10m
          timer_on_unit_inactive_sec: 24h
          service_exec_start: /usr/local/bin/backup.sh

License
-------

GPL-3.0-or-later
