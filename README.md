Role Name
=========

A brief description of the role goes here.

Requirements
------------

Docker installed on the target host

Role Variables
--------------

| Var Name           | Required | Default                               | Description            |
| ------------------ | :------: | ------------------------------------- | ---------------------- |
| `name`             | yes      |                                       | Network name to create |
| `driver`           | yes      |                                       | Setting network driver |
| `is_attachable`    | no       | False                                 | Setting `--attachable` |
| `remove`           | no       | False                                 | Remove network         |

Dependencies
------------

None

Example Playbook
----------------

    - hosts: servers
      roles:
         - role: docker_create_network
           name: test_network
           is_attachable: True

License
-------

BSD

Author Information
------------------

Mario Vejlupek
