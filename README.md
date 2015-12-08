[![Build Status](https://travis-ci.org/dpires/ansible-supervisor.svg)](https://travis-ci.org/dpires/ansible-supervisor)

ansible-supervisor
=========

An Ansible role for supervisor

Requirements
------------

N/A

Role Variables
--------------

 - `install_pip` Install pip dependency, defaults to `true`
 - `supervisor_name` The supervisor daemon name, defaults to `supervisord`
 - `supervisor_log_dir` The log directory, defaults to `/var/log/supervisor`
 - `supervisor_config_dir` The main config directory, defaults to `/etc/supervisor`
 - `supervisor_conf_dir` The conf directory, defaults to `/etc/supervisor/conf.d`
 - `supervisor_pid_dir` The directory to store the pid, defaults to `/var/run`


Dependencies
------------

```
 - dpires.pip
```

Example Playbook
----------------

```
    - hosts: all 
      roles:
         - { role: dpires.supervisor, install_pip: true }
```

License
-------

MIT

Author Information
------------------

David Pires
