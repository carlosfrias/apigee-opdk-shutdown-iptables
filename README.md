Apigee Shutdown IP Tables
==================================

This role shuts down iptables so that Apigee OPDK may be installed. 

Requirements
------------

The installation of Apigee OPDK requires root access. Credentials must also be supplied to override the empty placeholders
provided here. It is recommended that credentials be consolidated into a single credentials.yml file that can be stored 
separately. It is assumed that files containing credentials are stored in the ~/.apigee folder. 

Role Variables
--------------

None

Dependencies
------------

* opdk-setup-default-settings


Example Playbook
----------------

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
