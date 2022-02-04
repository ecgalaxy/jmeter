ECGALAXY Apache JMeter
======================

This Ansible role installs Apache JMeter.

Requirements
------------

In order to work JMeter requires a Java runtime present on the target machine.


Role Variables
--------------

- `jmeter_version: 5.4.1`: The version of JMeter to be installed.
- `jmeter_download_dir: "/tmp"`: The directory where JMeter is going to be downloaded.
- `jmeter_checksum: "sha512:..."`: The checksum of the specific tar.gz that has been chosen for the installation. This is available on the official website.
- `jmeter_install_dir: "/opt/jmeter/{{ jmeter_version }}"`: The place where JMeter is going to be installed.

Dependencies
------------

This role depends on the following ECGALAXY roles:

- ecgalaxy.common_packages

Example Playbook
----------------

    - hosts: all
      roles:
        - ecgalaxy.common_packages
        - ecgalaxy.jmeter

License
-------

Copyright the European Union 2022.

Licensed under the EUPL-1.2 or later.

Author Information
------------------

ECGALAXY team.
