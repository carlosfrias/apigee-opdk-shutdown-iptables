Apigee Shutdown IP Tables
==================================

This role shuts down iptables so that Apigee OPDK may be installed. 

Requirements
------------

This role runs if it is not executing inside of a Docker container.

Role Variables
--------------

ansible_virtualization_type: Populated by the setup module. 

Dependencies
------------

* opdk-setup-default-settings


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - hosts: '{{ hosts }}'
      become: yes
      
      roles:
        -  apigee-shutdown-iptables

License
-------

Apache License Version 2.0, January 2004

Author Information
------------------

Carlos Frias
