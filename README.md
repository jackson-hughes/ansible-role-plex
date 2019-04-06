[![Build Status](https://travis-ci.org/jhughes01/ansible-role-plex.svg?branch=master)](https://travis-ci.org/jhughes01/ansible-role-plex)

Ansible role: Plex
=========

This role installs and configures Plex Media Server.

Requirements
------------

The only additional step you will need to take after installing plex with this role is to ensure that port 32400/tcp (default) is opened. 

If you use firewalld, I have a simple role [here](https://github.com/jhughes01/ansible-role-firewalld), that will manage firewall ports for you.

Role Variables
--------------

This role currently supports 3 variables:

`plex_version`: The version of plex media server to install.
`plex_base_url`: The base url for the plex repository.
`plex_user_uid`: A variable allowing you to overwride the UID of the plex user.

Dependencies
------------

This role has no dependencies.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ansible-role-plex }

License
-------

GNU GPL v3

