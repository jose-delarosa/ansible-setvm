setvm
=====

This role runs some minimal configuration steps on VMs. This is not for general use, mostly for my own environment at work and home but could easily be adopted by anyone with minimal effort.

Tasks:

* Define repository to install packages from
* Install some packages I like to use which are not always installed
* Setup ntp
* For fun, display RAM and vCPU information
* [I'll add more as I think of useful tasks]

Requirements
------------

Though all tasks can be run on bare-metal hosts, I added some conditionals so it only runs on VMs, so get some VMs!

Role Variables
--------------

ntp_server

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- hosts: vms
  roles:
     - role: jose-delarosa.setupvm

License
-------

MIT

Author Information
------------------

jose.delarosa@dell.com
