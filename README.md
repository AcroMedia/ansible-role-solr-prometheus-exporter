Role Name
=========

This roles creates a systemd service for Prometheus solr exporter for a standalone solr server.

Requirements
------------

It is assumed that solr version >= 7 is installed on the server.

Role Variables
--------------

The variables that can be changed are :

* **prometheus_solr_exporter_installation_dir** (string) : This will be path to the solr installation directory. 
* **prometheus_solr_exporter_port** (int) : Port to listen to
* **prometheus_solr_exporter_solr_mode** (string) : Whether the installation is standalone or cloud.
* **prometheus_solr_exporter_solr_baseurl** (string) : Solr url eg: http://localhost:8983/solr
* **prometheus_solr_exporter_user** (string) : The user/owner of the solr dir
* **prometheus_solr_exporter_group** (string) : Group name of the solr dir
* **prometheus_solr_exporter_threads** (int) : Number of threads
* **prometheus_solr_exporter_conf_file** (string) : Config file path


Dependencies
------------

None 

Example Playbook
----------------

Including an example of how to use your role

    - hosts: servers
          roles:
             - { role: acromedia.solr-prometheus-exporter }

License
-------

GPLv3

Author Information
------------------

Chithra K, Acro Media Inc.
https://www.acromediainc.com/
