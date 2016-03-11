Rbenv ansible role
=========

Ansible role for system-wide installation of [rbenv](https://github.com/rbenv/rbenv) and rbenv [ruby-build](https://github.com/rbenv/ruby-build) plugin.

Requirements
------------

None.

Role Variables
--------------

	rbenv_version: v1.0.0
	rbenv_repo_path: https://github.com/rbenv/rbenv.git
	rbenv_ruby_build_repo_path: https://github.com/sstephenson/ruby-build.git
	rbenv_root_path: /usr/local/rbenv
	rbenv_ruby_version: 2.2.3

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
