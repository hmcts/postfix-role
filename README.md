Role Name
=========

Installing and configuring Postfix with TLS

Requirements
------------

Installs and configures postfix for MTA using TLS and turns selinux on with the default policy.
Copies the certificate files into a specified location, they are self signed for now.


Role Variables
--------------

Most values are configurable, this module install the certificates, for now they are self signed.
postfix_main_destinations: "all"
postfix_main_interfaces: "all"
postfix_main_protocols: "ipv4"
postfix_main_networks: "172.0.0.0/8"
postfix_tls_certs_dir: "/etc/pki/postfix/"
postfix_tls_key_location: "/etc/pki/postfix/tls.key"
postfix_tls_cert_location: "/etc/pki/postfix/tls.crt"

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: username.rolename, x: 42 }

License
-------
MIT

Author Information
------------------
HMCTS Reform Programme
