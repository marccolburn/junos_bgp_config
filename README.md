BGP Configuration
=========

Configure BGP for Junos.

Requirements
------------


Role Variables
--------------
bgp_asn: string
router_id: string
bgp_groups: list of dictionaries
* name: string
* type: external/internal, string
* local_address: string
* export_policy: str
* bfd: dictionary
** min: str
* neighbors: list of dictionaries
**address: str
**import: str

Dependencies
------------

N/A

Example Playbook
----------------

    - hosts: all
      roles:
         - { role: junos_bgp_config }

License
-------

BSD

Author Information
------------------

Marc Colburn Juniper
