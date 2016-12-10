Hopglass server
=========

[![Build Status](https://travis-ci.org/madonius/ansible-role-hopglass-server.svg?branch=master)](https://travis-ci.org/madonius/ansible-role-hopglass-server#)


Hopglass server installation for Debian

Requirements
------------

_Role_: [geerlingguy.nodejs](https://galaxy.ansible.com/geerlingguy/nodejs/)

Role Variables
--------------

##### Mandatory
| Name | Description |
| :--- | :--- | :--- |
| hopglass_config_file | The path for the configuration file |

##### Optional
| Name | Description |
| :--- | :--- |
| hopglass_aliases_file | The path for the hopglass aliases file |

##### Default
| Name | Default | Description |
| :--- | :--- | :--- |
| hopglass_home | "/var/lib/hopglass" | The home path for the hopglass user |
| hopglass_site | "default" | The name of the hopglass site |


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
        - role: madonius.hopglass_server
          hopglass_config_file: "~/ansible/hopglass/server/config.json"
          hopglass_aliases_file:"~/ansible/hopglass/server/aliases.json"
          hopglass_home:"/opt/hopglass/"
          hopglass_site:"gulasch"
```

License
-------

BSD

Author Information
------------------

Emmanouil Kampitakis [@madonius](https://twitter.com/Madonius)
