ECGALAXY Apache JMeter
=======================

This role installs Apache JMeter.

Requirements
------------

In order to work JMeter requires a java runtime present on the target machine.


Role Variables
--------------

- `jmeter_version: 5.4.1`: The version of JMeter to be installed.
- `jmeter_download_dir: "/tmp"`: The directory where JMeter is going to be downloaded.
- `jmeter_checksum: "sha512:bfc0faa84769b58c1fd498417b3a5c65749f52226bd6e3533f08ca7ea4a3798bb8d2cbd7091b443dd6837f3cbea5565c3c18e6497b40bec95616bf44dfdf590d"`: The checksum of the specific tar.gz that has been chosen for the installation. This is available on the official website.
- `jmeter_install_dir: "/opt/jmeter"`: The place where JMeter is going to be installed.

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

EUPL-1.2

Author Information
------------------

ECGALAXY team.
