Rbenv ansible role
=========
[![Build Status](https://travis-ci.org/spitfast/ansible-role-rbenv.svg?branch=master)](https://travis-ci.org/spitfast/ansible-role-rbenv)

Ansible role that installs [rbenv](https://github.com/rbenv/rbenv) and rbenv [ruby-build](https://github.com/rbenv/ruby-build) plugin for specified user.

Requirements
------------

Ansible version **2.0.1**

Role Variables
--------------
```yaml
---
rbenv_version: v1.0.0
rbenv_repo_path: https://github.com/rbenv/rbenv.git
rbenv_ruby_build_repo_path: https://github.com/sstephenson/ruby-build.git
rbenv_user: vagrant
rbenv_root_path: "/home/{{ rbenv_user }}/.rbenv"
rbenv_ruby_version: 2.3.1
```

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: localhost
  	  roles:
    	- rbenv

License
-------

MIT

Author Information
------------------

[Gordon Sumway](https://github.com/spitfast/)
