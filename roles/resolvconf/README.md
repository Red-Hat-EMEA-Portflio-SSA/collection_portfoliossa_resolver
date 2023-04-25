Role Name
=========

This is a 1 to 1 rebuild of: https://www.redhat.com/sysadmin/dns-configuration-ansible
It assures that Network Manager will not try to manage resolv.conf
Further i deploys it's own resolv.conf.

We could think of more sophisticated ways to manage resolver configuration, like injecting it into the connection definition (where it most likely came form), but we need to get things done...

Requirements
------------

Only makes sense on RH like systems with a Network Manager. This does not disable Network Manager nor is there a need to do so. 

Role Variables
--------------

We need following parameters set:
search_domain - optional, string variable with the search domain to be used
nameservers - mandatory, list of strings, each string is one Nameserver

Dependencies
------------



Example Playbook
----------------


License
-------

GPL

Author Information
------------------

Markus Schreier, Red Hat, mschreier@redhat.com
