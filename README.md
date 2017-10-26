Postgresql
===========

The purpose of this role is to install and configure postgresql.

Requirements
------------

Ensure that an up to date version of this role is available.

Role Variables
--------------

The default variables are stored in **defaults/main.yml** and are:

* packages_to_install:
* enabled_services:
* enabled_booleans:

Variables that should be set in either host or group vars are:

* pg_split_logs_and_data: This defaults to False in the role but can be overridden in a host or group var.
* pg_ver:
* postgresql_hba_entries:

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - name: Set up Postgres
      hosts: all
      become: True
      gather_facts: true

      roles:
        - postgresql

License
-------

MIT

Author Information
------------------

The Development Range Engineering, Architecture, and Modernization (DREAM) Team.
