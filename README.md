Create / Update / Delete tags
==========

Create, update or delete one or more tag of any ec2 resource.

Role Variables
--------------

Settable variables that are in defaults/main.yml.

* `resource`      : dictionary containing information about the resource
  * `id`          : id of the resource
  * `region`      : AWS region
  * `tags`        : dictionary containg the tags
  * `state`       : present to add tags, absent to delete them

Example Playbook
----------------

It assumes you use the ec2 dynamic inventory

```yaml
- hosts: localhost
  connection: local
  gather_facts: no
  roles:
    - role: create-tag
```

License
-------

GPL3
