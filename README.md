Role Name
=========

Installs minimal RabbitMQ 3.3.5 on CentOS 6.5

Requirements
------------

None.

Role Variables
--------------

Default:

* rabbitmq_management_plugin: true
* rabbitmq_remove_guest_user: false

You can override these values on your playbook.

Optional
You can also define optional variables:

# Create admin user

* rabbitmq_admin_user
* rabbitmq_admin_pass

# Create user for an application
* rabbitmq_app_user
* rabbitmq_app_pass
* rabbitmq_app_vhost

Dependencies
------------

* tcosta84.yum

Example Playbook
----------------

    - hosts: servers
      roles:
         - { role: tcosta84.rabbitmq }

License
-------

BSD

Author Information
------------------

This role was created by [Thiago Costa](http://thiagocostapy.com)
