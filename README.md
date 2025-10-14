prometheus_node_exporter
=======================

Install and run prometheus-node-exporter and open firewall for this service if needed

Requirements
------------

For RedHat OS family
EPEL repo (will be installed if not found)

Role Variables
--------------

*prometheus_ip* (optional), the ip of the prometheus host. \
Only used for RedHat OS family. \
When firewalld is running. \
If prometheus_ip is defined, the firewall will only allow queries to exporter from that host. \
If not, the firewall will allow exporter queries from all origins. \
When firewalld is not running, it is not configured. \

*port* (optional), the port prometheus service is listening to \
Only used for Debian OS family

*export_docker* (default false), if true docker metrics are gathered on *export_docker_port* (default: 9323)

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles
         - role: arikkert.prometheus_node_exporter
           prometheus_ip: 1.2.3.4
           port: 19100

License
-------

BSD

Author Information
------------------

    ARK-ICT
    Andre Rikkert de Koe - ICT
