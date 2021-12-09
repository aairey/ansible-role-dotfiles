aairey.dotfiles
===============


[![Build Status](https://travis-ci.org/aairey/ansible-role-dotfiles.svg?branch=master)](https://travis-ci.org/aairey/ansible-role-dotfiles)
[![ansible galaxy](https://img.shields.io/ansible/role/43968)](https://galaxy.ansible.com/aairey/dotfiles)
[![role downloads](https://img.shields.io/ansible/role/d/43968)](https://galaxy.ansible.com/aairey/dotfiles)



Installs aairey's dotfiles to the system for your user.

Based on [this gist](https://gist.github.com/aairey/a48a38d47f2bc2b8d03188dcc53eacaa).

Requirements
------------

Homebrew / Linuxbrew needs to be installed on the target system.

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: aairey.dotfiles }

Local building/testing
----------------------

You can test this role locally by running tox (see tox.ini file for the configuration).  
For example to run a test with Python 3.9 and Ansible 2.10, run:

```bash
# activate virtualenv which contains the test requirements
# or `pip install -r test_requirements.txt`
tox -e py39-ansible210
```

For more fine-grained test executions the different molecule commands can be used (`molecule lint`, `molecule converge`, ...) to save time in setting up the test env from scratch.

License
-------

GPL-3.0

Author Information
------------------

https://aairey.github.io/
