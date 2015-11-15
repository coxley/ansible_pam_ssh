coxley.pam_ssh
==============

Install and configure pam_ssh_agent_auth + sudo

This role is written to support many distributions but as of now only supports
Ubuntu and ArchLinux. Feel free to submit an issue or even better a PR if you
want it in your distro!

Configure
---------

Below are the configurable default variables:

```yaml

---                                     
pam_ssh_state: present                  
pam_ssh_keypath: %h/.ssh/authorized_keys

```

Requirements
------------

Managed node should have:

* openssh server (sshd)
* sudo

Dependencies
------------

For ArchLinux hosts, following roles are required from Galaxy:

* coxley.packer

License
-------

WTFPL

Author Information
------------------

Codey Oxley <codey.a.oxley+os@gmail.com>
