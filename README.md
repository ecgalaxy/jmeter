ECGALAXY Apache JMeter
======================

This Ansible role installs Apache JMeter.

Requirements
------------

- The `unzip` command, which can be provided by `ecgalaxy.common_packages`
- A Java runtime present on the target machine

Role Variables
--------------

- `jmeter_version`: The version of JMeter to be installed.
- `jmeter_download_dir`: The directory where JMeter is going to be downloaded.
- `jmeter_checksum:`: The checksum of the specific tar.gz that has been chosen for the installation. This is available on the official website.
- `jmeter_install_dir:`: The place where JMeter is going to be installed.

Dependencies
------------

- optional: ecgalaxy.common_packages

Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.bootstrap
        - ecgalaxy.common_packages
        - ecgalaxy.jmeter

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

ECGALAXY team.
