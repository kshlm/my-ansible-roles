kshlm.custom-rpms
=========
Installs all rpms in a given directory


Role Variables
--------------

Requires either (and only) one of the following variables to be set

- rpms_dir : A directory on the machine being configured that contains the rpms to be installed
- host_rpms_dir: A directory on the Ansible host that contains the rpms to be installed. The role syncs this directory with the machine being configured and installs the rpms.


Example Playbook
----------------

When the rpms are already present on the machine

```yml
---
- hosts: all
  vars:
    rpms_dir: /rpms
  roles:
    - kshlm.custom-rpms
```

When the rpms are on the host
```yml
---
- hosts: all
  vars:
    host_rpms_dir: ./rpms
  roles:
    - kshlm.custom-rpms
```

License
-------

MIT
