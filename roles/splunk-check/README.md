Role Name
=========

splunk-forwarder

Requirements
------------

Linux

Any pre-requisites that may not be covered by Ansible itself or the role should be mentioned here. For instance, if the role uses the EC2 module, it may be a good idea to mention in this section that the boto package is required.

Role Variables
--------------

  ansible_ssh_user: unixops
  ansible_ssh_private_key_file: /home/unixops/.ssh/unixops.pem
  ansible_ssh_extra_args: '-o UserKnownHostsFile=/dev/null -o StrictHostKeyChecking=no'
  force: 'false'
  
  # splunk latest version
  splunk_latest_rpm: splunkforwarder-{{splunk_major_ver}}-{{splunk_minor_ver}}-linux-2.6-x86_64.rpm
  # splunkforwarder-8.1.0.1-24fd52428b5a-linux-2.6-x86_64.rpm
  # splunkforwarder-8.1.1-08187535c166-linux-2.6-x86_64.rpm

Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: linux-check, x: 42 }

License
-------

BSD

Author Information
------------------

JCREW - AWS Operations Team


Role Tags
---------
check-version,
status,
installation,
deletion,
remove,
update,
enable-service,
start-service,

