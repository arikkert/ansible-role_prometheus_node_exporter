Role Name
=========

Install and run prometheus-node-exporter and open firewall for this service if needed

Requirements
------------

For RedHat OS family
EPEL repo (will be installed if not found)

Role Variables
--------------

*config_firewall*
Only used in RedHat os family
Default is false

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles
         - role: arikkert.prometheus_node_exporter
                 config_firewall: true

License
-------

BSD

Author Information
------------------

    ARK-ICT
    Andre Rikkert de Koe - ICT
