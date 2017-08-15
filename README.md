Role Name
=========

php71

Requirements
------------

This role is designed for EL 7 / CentOS 7

Role Variables
--------------

None

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: php71, tags: php71 }

If you require this role for your application you can use the following 'requirments.yml' lines to ensure the roles is downloaded and installed to your system. This assumes the template and your playbook uses the `svc_ansible` user.

requirments.yml
    # pull down common roles
      - src: git@code.bridgevine.io:ans-app/php71.git
        name: php71
        version: master
        scm: git

To install these roles use
    # ansible-galaxy install -r requirments.yml

License
-------

BSD
