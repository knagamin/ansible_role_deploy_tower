deploy_tower
=========

Deploy Ansible Tower automatically
* download the bundle installer
* deploy installer's inventory file with variables and a template
* kick setup.sh
* apply license via API endpoint

Requirements
------------

TODO

Role Variables
--------------
<!--
 FIXME: "eula_accepted": "true" must be needed in the license file for posting manually
 https://access.redhat.com/solutions/3065701
-->
license_file: location of the tower license file on control node.



Dependencies
------------
None

Example Playbook
----------------

    - hosts: tower_nodes
      roles:
         - { role: deploy_tower, license_file: license.txt }

License
-------

MIT

Author Information
------------------

Kiyo Nagamine

