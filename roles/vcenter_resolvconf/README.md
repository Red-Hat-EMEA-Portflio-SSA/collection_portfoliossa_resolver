Role Name
=========

This role reaches out to vcenter to change the resolver configuration of all ESXi hosts beloging to one cluster.

Requirements
------------

Only makes sens in VMware environment with vcenter and ESXi.

Role Variables
--------------

We need following parameters set:
search_domain - optional, string variable with the search domain to be used
nameservers - mandatory, list of strings, each string is one Nameserver
vcenter_cluster_name - name of the cluster the ESXi belong to.


Dependencies
------------
requires role: community.vmware 



Example Playbook
----------------


License
-------

GPL

Author Information
------------------

Markus Schreier, Red Hat, mschreier@redhat.com
