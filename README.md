Deploy User Role
=========

[![Build Status](https://travis-ci.org/mbreisch/deploy-user-role.svg?branch=master)](https://travis-ci.org/mbreisch/deploy-user-role)

Creates a deploy user, and sets ssh keys. Optionally, changes root password.

Requirements
------------

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

Variables:
* deploy_user_username: 
* deploy_user_password: ''
* deploy_user_new_root_password: ''

Defaults:
* deploy_user_change_root_password: yes
*     deploy_user_public_keys:
        - ~/.ssh/id_rsa.pub
  
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

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
