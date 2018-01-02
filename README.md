Rbenv ansible role
=========
An ansible role that installs [rbenv](https://github.com/rbenv/rbenv) and rbenv [ruby-build](https://github.com/rbenv/ruby-build) plugin for specified user.

Requirements
------------

Ansible version **2.0.1**

Role Variables
--------------
List of default variables. You can override variables in your playbook.
```yaml
---
rbenv_version: v1.0.0
rbenv_repo_path: https://github.com/rbenv/rbenv.git
rbenv_ruby_build_repo_path: https://github.com/sstephenson/ruby-build.git
rbenv_user: vagrant
rbenv_root_path: "/home/{{ rbenv_user }}/.rbenv"
rbenv_ruby_versions:
  - 2.4.2
rbenv_global_ruby_version: 2.4.2
rbenv_gems:
  - bundler
```

Dependencies
------------

None.

Installation
------------
add this to your requirements.yml
```yaml
- src: "https://github.com/rjlynch/ansible-role-rbenv"
  version: master
  name: rbenv-role
```

Example Playbook
----------------
```yaml
---
- hosts: localhost
  roles:
	- rbenv-role
```

License
-------

MIT

Author Information
------------------

[Gordon Shumway](https://github.com/spitfast/)
[Richard Lynch](https://github.com/rjlynch/)
