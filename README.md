role-wcl-nodejs
=============

Strongly inspired from Stouts.nodejs

Ansible role which manage nodejs and npm packages.


#### Variables

```yaml
nodejs_enabled: yes                       # The role is enabled

nodejs_repository: ppa:chris-lea/node.js  # NodeJS PPA or False for skip
nodejs_npm_modules: []                    # List modules which will be installed
```

#### Usage

Add `Stouts.nodejs` to your roles and set vars in your playbook file.

Example:

```yaml

- hosts: all

  roles:
    - role-wcl-nodejs

  vars:
    nodejs_npm_modules:
      - bower
      - jshint
```

#### License

Licensed under the MIT License. See the LICENSE file for details.

#### Feedback, bug-reports, requests, ...

Are [welcome](https://github.com/Stouts/Stouts.nodejs/issues)!

If you wish to express your appreciation for the role, you are welcome to send
a postcard to:

    Kirill Klenov
    pos. Severny 8-3
    MO, Istra, 143500
    Russia
